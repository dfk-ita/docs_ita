# I Gardens

In ogni regno, i Gardens sono il luogo dove depositare i tuoi LP per "coltivare" (farming) i token del potere. Nei giardini JEWEL di Serendale, i giocatori possono depositare LP per ricevere le emissioni di JEWEL, mentre negli Ice Gardens di Crystalvale ricevono le emissioni di CRYSTAL.

![](<../../.gitbook/assets/Cute Henry.gif>)

Inoltre, i giocatori possono assegnare i loro Eroi NFT a lavorare nei loro giardini. Questi eroi guadagnano ricompense aggiuntive in JEWEL o CRYSTAL in base all'abilità dell'eroe e all'importo investito nel giardino che stanno curando, quindi i giocatori che investono nei giardini e negli eroi hanno subito un'utilità sinergica per i loro NFT.

### Epoche ed Emissioni

Ogni token del potere ha il proprio programma di emissioni. In generale, le emissioni al minuto sono maggiori al lancio del token e diminuiscono nel tempo. Questa diminuzione delle emissioni non è lineare, quindi è importante rivedere i programmi delle emissioni per ciascun token nella relativa sottopagina dei Gardens.

Le emissioni sono regolate da periodi di tempo chiamati Epoche. Ogni token inizia nell'Epoca 1 al momento del lancio, che ha il tasso di emissione più alto. Con ogni Epoca, il tasso può cambiare o rimanere costante, come mostrato nella tabella di ogni token nella loro sottopagina dei Gardens.

Le epoche sulla blockchain Harmony sono legate alla velocità di blocco, quindi le emissioni di JEWEL sono legate alla velocità della catena Harmony e la lunghezza di ciascuna epoca (idealmente una settimana) può variare se la blockchain subisce rallentamenti.

Su Avalanche, le Epoche si basano su timestamp e durano esattamente una settimana.

### Allocazioni e ricompense

La quantità totale di ogni token emesso al minuto può essere determinata dalla Epoca, ma quei token devono andare da qualche parte! Ad ogni singolo giardino (che rappresenta una specifica coppia di LP) viene allocata una quota dei token totali coniati. L'assegnazione per ciascuna pool può essere visualizzata nella Seed Box. In base all'epoca attuale, al suo tasso di emissione e all'allocazione per una pool specifica, i giocatori possono determinare quanti gettoni verranno dati a quella pool ogni secondo, minuto o giorno. Da lì, la pool divide quei token tra tutti i suoi investitori proporzionalmente alla loro quota della pool totale e li distribuisce come ricompensa. Quando si effettuano questi calcoli è imperativo ricordare che i giocatori possono entrare o uscire liberamente dalle pool di liquidità, quindi la quota di ogni giocatore è costantemente in movimento man mano che la liquidità viene aggiunta o rimossa.

### Modello di Locking ( Blocco )

Per bilanciare gli elevati tassi di emissioni nelle epoche precedenti e per fornire stabilità dei prezzi, la nostra tokenomics include un modello di blocco sulle ricompense dei Gardens. Una parte dei token raccolti e distribuiti come ricompense dei giardini viene sbloccata. Una volta richiesti, questi token sbloccati vengono trasferiti direttamente nei portafogli dei giocatori e sono immediatamente utilizzabili. Tuttavia, una parte delle ricompense dei Giardini è bloccata nel sottosuolo. Queste ricompense vengono assegnate al portafoglio del giocatore, ma non è possibile accedervi o utilizzarle in alcun modo finché non vengono sbloccate.

Per ogni token, a partire dall'Epoca 1, il 5% delle ricompense richieste viene sbloccato mentre il 95% è bloccato. Ogni Epoca, la percentuale di ricompense che vengono sbloccate aumenta del 2%, quindi nella Epoca 2, il 7% è sbloccato e il 93% è bloccato, e così via. È importante notare che queste percentuali si basano sull'Epoca nel momento in cui il giocatore sceglie di ritirare le ricompense, non quando sono state assegnate. Se un giocatore sceglie di non prelevarle subito, la percentuale che potrà ritirare aumenta del 2% ogni Epoca. Una volta che un giocatore ha prelevato, il resto delle ricompense bloccate smette di essere sbloccato fino all'Epoca 51, a quel punto iniziano a sbloccarsi linearmente nelle 52 Epoche successive. Dopo l'Epoca 51, non si verificheranno ulteriori blocchi e tutte le ricompense appena generate verranno completamente sbloccate subito.

### Modello di Locking  - Sblocco anticipato con gli Eroi NFT

Una delle caratteristiche più uniche di DeFi Kingdoms sono i nostri Eroi NFT che forniscono una vera utilità in-game. La professione di mining è uno di questi casi d'uso. I giocatori che hanno ricompense bloccate possono inviare i loro Eroi in missioni di mining JEWEL o CRYSTAL per sbloccarne alcuni in anticipo, garantendo l'accesso a ricompense bloccate prima dell'Epoca 51 e sbloccandole più velocemente anche una volta raggiunta quella soglia. Non tutti gli eroi avranno lo stesso livello di competenza nel mining, quindi è importante conoscere le varie statistiche utilizzate dagli eroi e come funziona ogni professione quando si cerca di acquistarli e utilizzarli.

### Commissioni di deposito e prelievo dei Gardens

**Non ci sono commissioni di deposito per lo staking di token LP nei Giardini**. Per proteggerci da prestiti flash e pump and dump, abbiamo implementato commissioni di prelievo per il ritiro di token LP in staking. Ogni prelievo azzera il timer della commissione. Le commissioni di prelievo sono elencate di seguito:

* **0.01%** se un utente preleva dopo **4 Epoche**
* **0.25%** se un utente preleva dopo  **2 Epoche ma prima di 4 Epoche**
* **0.5%** se un utente preleva dopo **5 giorni ma prima di 2 Epoche**
* **1%** se un utente preleva prima di **5 giorni. \***
* **2%** se un utente preleva prima di **3 giorni. \***
* **4%** se un utente preleva prima di **24 ore. \***
* **8%** se un utente preleva prima di **1 ora. \***
* **25%** se un utente preleva **durante lo stesso blocco.**

_\*Nel caso di JEWEL e Harmony, i giorni e le ore elencati presuppongono una velocità di blocco di 2 secondi durante tale periodo e dipenderanno dalla velocità della blockchain_.

## ****
