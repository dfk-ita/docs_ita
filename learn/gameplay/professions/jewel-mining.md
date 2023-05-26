---
description: Informazioni riguardanti le missioni di Token Mining
cover: ../../../.gitbook/assets/pickmankhudmire (1).webp
coverY: 0
---

# Token Mining

Le missioni di Token Mining possono essere svolte da un massimo di sei Eroi alla volta in ogni regno. Queste missioni sbloccano [Power Tokens](../../../come-funziona-defi-kingdoms/i-token-del-potere/#power-tokens) dal saldo bloccato e possono assegnare altri oggetti rari.

> _Siete pronti ad iniziare a scavare per trovare un vero tesoro? Andiamo! Ti offro un po' di birra se torniamo vivi!_

Le missioni di Token Mining si iniziano nella Zona delle **Professioni** parlando con il **Miner** o il **Pickman**, a seconda del regno. Gli Eroi possono iniziare le missioni di Token Mining solo se il giocatore ha un saldo bloccato di Power Tokens del regno. Il rendimento dei tokens aumenta con il saldo bloccato del giocatore fino ad un limite specifico.

Tutti gli Eroi possono tentare le Missioni di Token Mining, ma gli Eroi con il **gene della professione Mining** useranno la loro Stamina in modo più efficiente ed avranno maggiori possibilità di ottenere le ricompense degli oggetti. Completare con successo una Missione di Token Mining garantirà ad ogni Eroe una piccola quantità di XP ed una possibilità di aumentare la propria **abilità nella professione Mining**.

Queste missioni hanno anche la possibilità di ricompensare gli Eroi con **Gaia's Tears**, **Rune** e **Yellow Pet Eggs**. Tutti questi oggetti possono essere scambiati con altri tokens o oggetti presso il Trader nel [Marketplace](../marketplace.md). Alcuni oggetti sono utilizzati anche come reagenti per **Pozioni** e [Enhancement Stones](../heroes/enhancement-stones.md), per far nascere [Pets](../heroes/pets.md) e per far [salire di livello gli Eroi](../heroes/leveling.md).

### Le Basi delle missioni di Mining

#### Durata per Stamina

12 minuti (10 con il **gene della professione Mining**)

#### Stamina Richiesta

1 Stamina minimo

#### Numero di Eroi Richiesti

1-6 Eroi

### Ricompense Tokens

Le **missioni di Token Mining** richiedono che il giocatore selezioni un **Miner Leader** per ogni missione, le cui statistiche determinano la quantità massima di Power Tokens che possono essere sbloccati durante la missione. Queste statistiche includono i punteggi di **Forza(STR)** e **Resistenza(END)** dell'Eroe, la sua abilità nel **Mining** ed il possesso del **gene della professione Mining**. È possibile aggiungere fino a cinque Eroi per assistere il minatore leader, le cui statistiche determinano la ricompensa finale della missione. Se la somma totale sbloccabile del gruppo raggiunge il massimo, l'aggiunta di altri Eroi non aumenterà ulteriormente le ricompense in tokens, anche se questi Eroi potranno comunque ricevere ricom**pense in oggetti**.

#### Formula

La ricompensa in Power Tokens sbloccati per il Mining per ogni stamina spesa è pari al **`MaxUnlockRate`** o alla somma del **`HeroUnlockRate`** per ogni Eroe inviato nella missione, a seconda di quale valore sia minore.

Questi valori sono calcolati in base alle seguenti formule e variabili:

* **`maxUnlockRate`** - La quantità massima di Power Tokens che possono essere sbloccati per ogni Stamina spesa. Questa quantità viene impostata in base alle statistiche del **Miner Leader**:\
  `maxUnlockRate = (1000 * (0.25 + (`**`STR`**`+`**`END`**`) * 0.000625 + (`**`MinSkl`**`) * 0.0025)) /`` `**`lockedRatio`**
* **`heroUnlockRate` -** La quantità di Power Tokens che vengono sbloccati per ogni Stamina spesa. Questa quantità è calcolata in base alle statistiche di **ogni minatore**:\
  `heroUnlockRate = (1000 * (0.25 + (`**`STR`**`+`**`END`**`) * 0.000625 + (`**`MinSkl`**`) * 0.0025)) / (6 * (1000 - 166 *`` `**`geneBonus`**`))`
* **`lockedRatio`** - Il ratio tra **`minLocked`** e **`lockedPT`**:

```javascript
if lockedPT > minLocked {
    lockedRatio = (1000 - 166 * geneBonus)
else
    lockedRatio = ((1000 - 166 * geneBonus) * minLocked) / lockedPT
}
```

* **`lockedPT`** - Il numero di Power Tokens bloccati nel portafoglio del giocatore.
* **`minLocked`** - La quantità minima di Power Tokens bloccati che un giocatore deve possedere per ottenere la massima ricompensa mineraria. Impostato a `5000` Power Tokens.
* **`STR`** / **`END`** - I valori delle Statistiche STR e END dell'Eroe
* **`MinSkill`** - **L'abilità di Mining dell'Eroe**, arrotondata per difetto (ad esempio, usare 15 per 15,9 Mining).
* **`geneBonus`** - Se un Eroe possiede il **gene della professione Mining**, questo fornisce un bonus del 20% ai rendimenti in Power Tokens, aumenta le possibilità di trovare Gaia's Tears e le Rune, e diminuisce il tempo speso per la missione di Token Mining da 12 minuti a 10 minuti per punto Stamina speso. Se l'Eroe ha questo gene, **`geneBonus`**`= 1`, atrimenti, **`geneBonus`**`= 0`.

#### Jackpot Mining

Per ogni 15 Stamina spesi dal **Miner Leader**, il giocatore riceverà un tiro bonus con una probabilità del 10% di sbloccare Power Tokens bonus. Il bonus massimo è di 10PT se il portafoglio ha almeno 1.250 Power Tokens bloccati. Il bonus diminuisce linearmente se il portafoglio ha meno di 1.250 Power Tokens bloccati e si dimezza se il **Miner Leader** non ha il **gene della professione Mining**.

### Ricompense Oggetti

{% hint style="info" %}
Le percentuali di caduta degli oggetti riportate di seguito aumentano in base a diverse combinazioni delle statistiche di Forza(STR) e Resistenza(END) dell'Eroe, della sua abilità di Mining e della presenza del gene della professione Mining.
{% endhint %}

<table><thead><tr><th width="224.69851729818782">Nome</th><th width="175">Drop Rate Base</th><th width="153">Ricompensa XP</th><th>Stamina Richiesta</th><th data-hidden align="center"> </th></tr></thead><tbody><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/gaias-tear.png" alt="" data-size="original"> Gaia's Tear</td><td>7.5% / 11.25% *</td><td>10 XP</td><td>Possibilità Drop ogni <strong>5</strong> punti Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/shvas-rune.gif" alt=""> Shvās Rune</td><td>0.3% / 1.5% *</td><td>30 XP</td><td>Possibilità Drop ogni <strong>5</strong> punti Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/moksha-rune.gif" alt=""> Moksha Rune</td><td>0.009% / 0.045% *</td><td>100 XP</td><td>Possibilità Drop ogni <strong>5</strong> punti Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-yellow.png" alt="Green Pet Egg"> Pet Egg Giallo</td><td>0.02%</td><td>100 XP</td><td>Possibilità Drop ogni <strong>10</strong> punti Stamina</td><td align="center"><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-green.png" alt="Green Pet Egg"></td></tr></tbody></table>

_\*La percentuale più alta si applica agli Eroi con il **gene della professione Mining**_.





