---
description: Informazioni riguardanti le missioni di Gardening
cover: ../../../.gitbook/assets/gardener-splash.428a0e2f.gif
coverY: 0
---

# Gardening

Le **Missioni di Gardening** possono essere svolte da un massimo di due Eroi alla volta in ciascuna delle pool di liquidità incentivate elencate nella **Seed Box** situata nella zona **Gardens**. Queste missioni assegnano **Power Tokens** e **JEWEL**, oltre a **Piante** ed altri oggetti rari.

> Un amico dei giardini è un mio amico. Ti prego, lascia che ti mostri le nostre strade. Insieme, possiamo coltivare un bellissimo campo.

Le Missioni di Gardening si iniziano nella zona **Professions** e parlando con il **Greenskeeper**. Gli Eroi possono dedicarsi al Gardening in tutti i giardini disponibili, ma le ricompense in **Power Tokens** e **JEWEL** aumentano solo in quelli in cui il giocatore ha piantato i semi (depositato tokens LP nelle pool incentivate), e la resa in tokens aumenta insiem al numero di semi piantati dal giocatore in quel particolare giardino.

Le Missioni di Gardening hanno anche la possibilità di ricompensare gli Eroi con **Piante**, **Gaia's Tears**, **Rune** e **Green Pet Eggs**, indipendentemente dal fatto che il giocatore abbia o meno semi(LP) nel Garden dove si svolge la missione. Tutte le Piante possono essere vendute presso il Vendor nel [Marketplace](../marketplace.md) in cambio di **Gold** o scambiate grazie al Trader con altri tokens o oggetti. Alcune Piante sono reagenti per **Pozioni** ed [Enhancement Stones](../heroes/enhancement-stones.md), mentre altre sono usate per far nascere [Pets](../heroes/pets.md).

## **Le Basi delle missioni di Gardening**

#### Durata per punto Stamina

12 minuti (10 con **Gardening come gene di professione**)

#### Stamina Necessaria

1 punto Stamina minimo

#### Eroi Richiesti per Missione

1-2 Eroe per Giardino

## **Token Rewards**

Il primo Eroe inviato a fare una missione in ogni Giardino sarà ricompensato in **Power Tokens** del regno, mentre il secondo Eroe guadagnerà **JEWEL**. Queste ricompense sono finanziate dal portafoglio [Quest Reward Fund](https://subnets.avax.network/defi-kingdoms/address/0x1137643FE14b032966a59Acd68EBf3c1271Df316) di ogni regno. I rendimenti dei Giardini dipendono in larga misura dalla quota del giocatore delle **Liquidity Pools** in cui lavoreranno i suoi Eroi, dall'equilibrio generale del Quest Reward Fund e dalle statistiche degli Eroi in missione. Di conseguenza, ci sarà una grande variazione nei rendimenti tra i giocatori e le Liquidity Pools, così come una variazione nei rendimenti nel tempo, man mano che il Quest Reward Fund cresce o si riduce.

### Formula

Le ricompense tokens delle Missioni di Gardening utilizzano la seguente formula, che si applica sia alle ricompense in Power Tokens che a quelle in JEWEL, quando applicabili.

`earnRate (per stamina spent) =`**`annealingFactor`**`* (`**`rewardPool`**`*`**`poolAllocation`**` `_`*`_**`LPowned`**`* (0.1 + (`**`WIS`**`+`**`VIT`**`) / 1222.22 +`**`GrdSkl`**`/ 244.44)) / (43,200 - (7200 *`**`geneBonus`**`))`

Calcolato da queste variabili:

* **`annealingFactor` ** - Un moltiplicatore applicato al momento del lancio che diminuisce gradualmente nel tempo, permettendo al Quest Fund di continuare a crescere. **`annealingFactor`** inizia a `50` e diminuisce ogni due settimane fino ad un  minimo di `1` dopo 26 settimane.
  * **`annealingFactor`**` ``= (9100 - 49 * (`**`daysSinceLaunch`**`/ 14) * 14) / 182`
  * Ai fini del calcolo **`daysSinceLaunch`**, le Missioni di Gardening su Crystalvale e Serendale sono state rilasciate il 15/09/2022.
* **`rewardPool` ** - Il relativo saldo dei tokens nel [Quest Reward Fund](https://subnets.avax.network/defi-kingdoms/address/0x1137643FE14b032966a59Acd68EBf3c1271Df316).&#x20;
* **`poolAllocation` ** - La percentuale di emissioni di tokens assegnata al Giardino specifico (in decimali, ad esempio 0,1 per il 10%).
* **`LPowned` ** - La percentuale della Pool di liquidità che il giocatore possiede nel Giardino selezionato (in decimali, ad esempio 0,0015 per 0,15%).
* **`WIS`** / **`VIT`** - Il valore delle statistiche di **Wisdom** e **Vitality** dell'Eroe.
* **`GrdSkl` ** -  Il livello professionale di **Gardening** dell'Eroe, arrotondata per difetto (ad esempio usa 15 per 15,9).
* **`geneBonus` ** - Se un Eroe possiede il gene della professione Gardening, questo fornisce un bonus del 20% ai rendimenti dei tokens, aumenta le possibilità di trovare Gaia's Tears e Rune e diminuisce il tempo trascorso a fare Gardening per Stamina da 12 minuti a 10 minuti. Se l'Eroe possiede questo gene, **`geneBonus=1`**, altrimenti **`geneBonus=0`**.

### Ricompense Minime

La Ricompensa Minima in tokens guadagnata per ogni punto Stamina speso è di 0.0002. Se **`earnRate`** è inferiore a questa soglia, verrà aumentato a 0.0002.

Le Ricompense Minime sono attive solo quando nel Quest Reward Fund sono disponibili almeno 420.000 tokens del tipo appropriato.

### Gardening Jackpots

Per ogni 15 punti Stamina spesi durante la missione, il giocatore riceverà un tiro bonus con una probabilità del 9,9% di ricevere 0.1 token bonus ed una probabilità del 0.1% di ricevere un ulteriore token bonus. Questo bonus si dimezza se l'Eroe non ha il **gene della professione Gardening.** I giocatori non possono ricevere entrambi i bonus contemporaneamente.

I premi Jackpot sono attivi solo quando nel Quest Reward Fund sono disponibili almeno 950.000 tokens del tipo appropriato.

### **Ricompense Oggetti**

{% hint style="info" %}
Le percentuali di drop degli oggetti riportate di seguito aumentano in base a diverse combinazioni delle statistiche di Saggezza (WIS) e Vitalità (VIT) dell'Eroe, del suo livello di Gardening e della presenza del gene della professione Gardening.
{% endhint %}

|                            Oggetto                            |      Drop Rate Base      |   Ricompensa XP   |                Stamina Richiesta                |
| :-----------------------------------------------------------: | :----------------------: | :---------------: | :---------------------------------------------: |
|   ![](<../../../.gitbook/assets/image (6) (1).png>)Bluestem   |       <p><br>9%</p>      |  <p><br>10 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
|    ![](<../../../.gitbook/assets/image (5).png>)Spiderfruit   |       <p><br>6%</p>      |  <p><br>10 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
| ![](<../../../.gitbook/assets/image (2) (1) (1).png>)Milkweed |       <p><br>4%</p>      |  <p><br>10 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
|   ![](<../../../.gitbook/assets/image (11).png>)Gaia's Tear   | <p><br>7% - 11.25% *</p> |  <p><br>10 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
|  ![](<../../../.gitbook/assets/image (3) (1).png>) Runa Shvās | <p><br>0.3% - 1.5% *</p> |  <p><br>30 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
|    ![](<../../../.gitbook/assets/image (4).png>)runa Moksha   |    0.009% - 0.045% \*    | <p><br>100 XP</p> | <p>Possibilità Drop ogni<br>5 punti Stamina</p> |
|  ![](<../../../.gitbook/assets/image (8) (2).png>)Uovo Verde  |     <p><br>0.02%</p>     | <p><br>100 XP</p> |      Possibilità Drop ogni 10 punti Stamina     |

* La percentuale più alta si applica agli Eroi con il **gene della professione Gardening**.
