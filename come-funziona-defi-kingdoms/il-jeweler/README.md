---
cover: ../../.gitbook/assets/Screen Shot 2022-11-04 at 9.09.48 AM.png
coverY: 0
---

# Il Jeweler

Jeweler 2.0

Il **Jeweler 2.0** adotta i vantaggi ottenuti dal modello di governance **veToken** sviluppato da [Curve](https://curve.fi/#/ethereum/swap) e li combina con un metodo per la distribuzione delle commissioni, i premi airdrop ed i [Power-Ups](power-ups.md) in-game. **cJEWEL** è il nome del token di **governance** in Crystalvale e **sJEWEL** è l'equivalente di Serendale (entrambi funzionalmente sono uguali, anche se questi documenti utilizzeranno cJEWEL per comodità).

{% hint style="info" %}
Il modello Jeweler 2.0 è stato adottato con una [votazione governance della Community](https://vote.defikingdoms.com/#/proposal/0x8b74fefcfbd5b6751c190361577fd65ff79084b5250ed3265a14a16140d67fba) tenuta il 14/10/2022 ed è entrata in vigore il 4/11/2022. Ha sostituito il modello [Jeweler 1.0](./#jeweler-1.0) che utilizzava xJEWEL e xCRYSTAL.
{% endhint %}

I giocatori ricevono tokens cJEWEL o sJEWEL **bloccando i loro JEWEL** nel Jeweler del reame applicabile per un periodo di tempo a loro scelta. Questo meccanismo di blocco incoraggia lo staking nel protocollo e consente a coloro che desiderano supportare il progetto a lungo termine di avere più voce in capitolo e ricevere una quota maggiore dei premi. Scoraggia inoltre le terze parti dal voto di gioco e dagli snapshot acquistando grandi quantità di JEWEL subito prima, solo per venderli subito dopo.

I token cJEWEL/sJEWEL sono **legati all'anima del portafoglio che li genera (soulbound)** e non possono essere trasferiti o scambiati. I giocatori possono tenere i loro cJEWEL/sJEWEL dopo la scadenza del periodo di blocco e continuare a ricevere ricompense e potere di governance.

## Benefici del detenere

I quattro principali vantaggi del detenere cJEWEL sono: governance, distribuzione delle commissioni, miglioramenti in-game e accesso a funzionalità premium [(Power-Up)](power-ups.md), e blocco dei token.

* La [governance](./#votazioni-governance) utilizzerà l'equilibrio cJEWEL/sJEWEL degli utenti per votare le proposte.
* I premi arriveranno attraverso la [distribuzione delle commissioni](./#benefici-del-detenere-cjewel), ma anche aidrops regolari possono essere implementati grazie alla natura timelock più sicura di cJEWEL/sJEWEL.
* I [potenziamenti in-game (Power Ups)](./#power-ups) consentiranno ai giocatori di allocare una certa quantità di cJEWEL/sJEWEL per ottenere l'accesso ai bonus, miglioramenti e funzionalità premium.
* A causa del fatto che cJEWEL e sJEWEL richiedono un certo periodo di blocco del token **JEWEL** per essere creati, il risultato atteso di questo sistema è una riduzione complessiva del supply liquido disponibile di JEWEL (a seconda del coinvolgimento dell'utente con il sistema).

## Meccanismo di Blocco

I giocatori possono bloccare i propri JEWEL nello smart contract del Jeweler per un periodo di tempo compreso tra 7 giorni e 1095 giorni (3 anni). In cambio riceveranno un importo di cJEWEL/sJEWEL relativo alla quantità di token bloccati e alla durata del tempo di blocco scelto, secondo questa formula, dove MAX DAYS è pari a 1095 e daysLocked è un minimo di 7:

<figure><img src="../../.gitbook/assets/Screenshot 2022-11-11 alle 17.59.24.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Esempio:**

![](<../../.gitbook/assets/image (10) (1).png>)Keal ha 50.000 JEWEL e vuole depositarli nel Jeweler. Decide di depositare con il periodo di blocco minimo di 7 giorni e riceve \~320 cJEWEL.

![](<../../.gitbook/assets/image (11) (1).png>)Rolando non ha gli stessi mezzi di Keal, ma decide di rimediare depositando e bloccando più a lungo i suoi JEWEL. Non volendo essere superato da Keal, acquisisce 320 cJEWEL depositando \~960 JEWEL per un anno.

**Resoconto:**

_Non devi avere più JEWEL per avere la massima influenza con questo modello._
{% endhint %}

I giocatori possono ricevere più cJEWEL senza depositare più JEWEL **estendendo il periodo di blocco**. Possono anche **aggiungere più JEWEL** a ciò che è già bloccato (utilizzando lo stesso tempo rimanente bloccato) per ricevere più cJEWEL. I premi possono essere richiesti manualmente, ma verranno anche automaticamente richiesti quando un giocatore effettua un deposito aggiuntivo, estende il periodo di blocco o ritira il proprio saldo JEWEL.

## Prelievi

Quando i giocatori ritirano JEWEL dal contratto cJEWEL, possono prelevare **solo il 100% del saldo**. Ciò significa che tutti i cJEWEL verranno bruciati ogni volta che un giocatore esegue questa azione.

{% hint style="danger" %}
**Prelievo di Emergenza**

Se il periodo di blocco non è scaduto, i giocatori possono ritirarsi solo utilizzando il metodo di **Prelievo di Emergenza**, che **restituirà il 50% del saldo bloccato e brucerà il restante 50%**.
{% endhint %}

## Interazioni col Jeweler

Questo modello cambia il modo in cui i giocatori interagiranno con il Jeweler, consentendo loro di utilizzare le seguenti funzioni:

* **`CreateLock (Crea Blocco)`**— (Disponibile solo se si possiede 0 cJEWEL) Selezionare una quantità di JEWEL da depositare e giorni da bloccare per ricevere cJEWEL in cambio in base ai valori scelti.
* **`IncreaseAmount (Incremento Deposito)`** — Consente di aggiungere più JEWEL al saldo depositato e ricevere più cJEWEL in base al programma di blocco rimanente per il saldo esistente.
* **`IncreaseUnlockTime (Incremento del Tempo di Sblocco)`** — Permette di ricevere cJEWEL estendendo il periodo di sblocco del tuo saldo JEWEL esistente.
* **`ClaimReward (Reclama Ricompense)`** — Consente di reclamare eventuali premi di compartecipazione alle commissioni del Jeweler.
* **`UpdatePool (Aggiorna Pool)`**— Aggiorna i premi disponibili derivanti da cJEWEL per tutti prelevando le commissioni dal contratto _FeeCollector_ (questo viene anche utilizzato ogni volta che qualcuno deposita, estende i periodi di sblocco, reclama premi o preleva).
* **`Withdraw (Prelievo)`**— Consente di prelevare l’intero saldo JEWEL dal Jeweler se il periodo di blocco è terminato.
* **`EmergencyWithdraw`** **`(Prelievo d’Emergenza)`**— Consente di prelevare prima della scadenza del periodo di blocco, ma con una penale del 50% (che viene bruciata).

## Votazioni Governance

Come molti progetti DeFi, gli sviluppatori di DeFi Kingdoms possono chiedere votazioni governance per autorizzare i possessori di token a prendere decisioni sulla direzione del progetto. Le votazioni governance potrebbero determinare l'inclusione di un nuovo token tra le pool incentivate, il ritiro di un token dalle pool o un cambiamento di policy che influisca sui detentori di tokens.

Quando ciò accade, la votazione viene annunciata su Discord e tramite gli altri accounts social media di DeFi Kingdoms. I possessori di cJEWEL e sJEWEL possono visitare il portale [Governance](https://vote.defikingdoms.com/#/), dove possono collegare il proprio wallet ed esprimere un numero di voti pari al numero di tokens posseduti.

Le votazioni governance consentono ai detentori del token di avere una voce attiva nel processo decisionale e gli sviluppatori lo considerano una componente chiave per un progetto DeFi di successo.

{% hint style="info" %}
Oltre ai titolari di cJEWEL e sJEWEL, anche i titolari di Eroi NFT e Lands NFT hanno diritto di voto.

Gli Eroi NFT hanno un potere di voto di 10 cJEWEL/sJEWEL come risultato di una [votazione governance della Community](https://vote.defikingdoms.com/#/proposal/0xd74484526e93cd325e853aea1444d0c6d3019749beb31b65ee03f1a52e18e04f) tenutasi il 23/02/2022 e le Lands NFT hanno un potere di voto di 100 token cJEWEL/sJEWEL.
{% endhint %}

## Distribuzione delle Commissioni

Una parte delle commissioni di transazione raccolte nel gioco viene inviata al Jeweler come ricompensa per i depositanti. Ciò include 1/6 delle commissioni raccolte dal DEX ed il [15% delle commissioni Power Token dalle transazioni in-game](../i-token-del-potere/#transazioni-e-ricompense), incluse evocazioni di Eroi, incubazioni di Pets, vendita di Eroi, Pets e Lands, e livellaggio di Eroi.

Queste commissioni sono vendute per JEWEL e matureranno per il giocatore in base alla loro quota del totale di cJEWEL/sJEWEL in circolazione e saranno richiedibili in qualsiasi momento, in modo simile a come funzionano i [Gardens](../the-gardens/). Poiché la quantità di tokens che entrano in questo montepremi oscilla in base al volume delle transazioni e poiché la quota di ogni giocatore oscilla con depositi e prelievi, il Jeweler non ha un APR fisso.

{% hint style="info" %}
Poiché le commissioni maturano e vengono distribuite separatamente su ciascun reame, i premi cJEWEL e sJEWEL differiranno in base al volume delle transazioni in Crystalvale e Serendale. I giocatori dovrebbero scegliere con attenzione dove e per quanto tempo puntare i loro JEWEL.
{% endhint %}

La richiesta delle ricompense può essere effettuata manualmente in qualsiasi momento ed avverrà anche automaticamente ogni volta che il giocatore deposita più JEWEL, estende il tempo di blocco o ritira il proprio saldo JEWEL.

Per maggiori dettagli su come queste commissioni vengono ripartite tra i titolari di token, vedere [questo articolo](https://dev.to/heymarkkop/understanding-sushiswaps-masterchef-staking-rewards-1m6f).

## Power-Ups

I possessori di cJEWEL/sJEWEL potranno attivare **miglioramenti di gioco e ricompense** destinando una parte dei loro possedimenti all'attivazione. I [Power-Ups](power-ups.md) utilizzano il tuo "saldo di potenziamento disponibile", che è la quantità totale di cJEWEL che detieni meno i requisiti cJEWEL di ciascuno dei tuoi potenziamenti attivi. L'attivazione dei Power-Up non consuma cJEWEL o i JEWEL utilizzato per produrli. I potenziamenti possono essere disattivati ​​in qualsiasi momento, o automaticamente, se il saldo cJEWEL del giocatore scende al di sotto del minimo necessario per mantenerli attivi.

I premi Power-Up possono includere bonus all'esperienza dell'Eroe, commissioni di gioco ridotte e accesso a funzionalità premium. Questi potenziamenti verranno implementati nel tempo dopo il rilascio di cJEWEL.

{% content-ref url="power-ups.md" %}
[power-ups.md](power-ups.md)
{% endcontent-ref %}

### Contract Addresses

* cJEWEL (DFK Chain): [`0x9ed2c155632C042CB8bC20634571fF1CA26f5742`](https://subnets.avax.network/defi-kingdoms/address/0x9ed2c155632C042CB8bC20634571fF1CA26f5742)
* sJEWEL (Klaytn): [`0xaA8548665bCC12C202d5d0C700093123F2463EA6`](https://scope.klaytn.com/token/0xaa8548665bcc12c202d5d0c700093123f2463ea6)



## Jeweler 1.0

Il Jeweler 1.0 è stato adattato dal contratto [SushiBar](https://docs.sushi.com/docs/Products/Yield%20Farming/The%20SushiBar) di [SushiSwap](https://www.sushi.com/), che ha consentito ai giocatori di depositare rispettivamente su JEWEL e CRYSTAL per ottenere xJEWEL e xCRYSTAL. Una parte delle commissioni di gioco raccolte è stata scambiata con il Power Token, aumentando il rapporto tra il Power Token e l'xToken.

Quando il giocatore prelevava, scambiava il proprio xToken con il Power Token. Più a lungo avevano detenuto l'xToken, più il rapporto sarebbe aumentato, e quindi più Power Token ricevevano rispetto ai loro depositi.

### Contract Addresses

#### Harmony

* xJEWEL: [`0xA9cE83507D872C5e1273E745aBcfDa849DAA654F`](https://explorer.harmony.one/address/0xA9cE83507D872C5e1273E745aBcfDa849DAA654F)

#### DFK Chain&#x20;

* xCRYSTAL: [`0x6e7185872bcdf3f7a6cbbe81356e50daffb002d2`](https://subnets.avax.network/defi-kingdoms/address/0x6e7185872bcdf3f7a6cbbe81356e50daffb002d2)
* xJEWEL: [`0x77f2656d04E158f915bC22f07B779D94c1DC47Ff`](https://subnets.avax.network/defi-kingdoms/token/0x77f2656d04E158f915bC22f07B779D94c1DC47Ff)
