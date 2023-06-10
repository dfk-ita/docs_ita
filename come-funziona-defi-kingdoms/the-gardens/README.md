# I Giardini

In ogni Regno, i Giardini sono il luogo in cui depositare i token delle pool di liquidità (qui indicati come "tokens LP") per ricevere una quota di emissioni di [Power Token](../i-token-del-potere/#power-tokens). Nei [Giardini JADE](giardini-jade.md) di Serendale, i giocatori possono depositare per ricevere le emissioni di JADE, mentre nei [Giardini CRYSTAL](ice-gardens.md) di Crystalvale sono in palio emissioni di CRYSTAL.

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

Inoltre, i giocatori possono assegnare i loro Eroi NFT a lavorare nei loro Giardini attraverso [Missioni di Gardening](../../learn/gameplay/professions/gardening.md). Quegli Eroi guadagnano ricompense aggiuntive in JEWEL e JADE o CRYSTAL in base al Regno dove si esegue la Missione, all'abilità degli Eroi ed alla quantità di tokens LP depositati nel Giardino che stanno curando, quindi i giocatori che depositano tokens LP nei Giardini ed assegnano Eroi in quegli stessi Giardini, hanno un'utilità sinergica tramite per i loro NFT.

### Epoche ed Emissioni

Inoltre, i giocatori possono assegnare i loro [Eroi](../the-heroes.md) NFT a lavorare nei loro Giardini attraverso le Missioni di [Gardening](../../learn/gameplay/professions/gardening.md). Questi Eroi guadagnano ricompense aggiuntive in JEWEL, CRYSTAL o JADE in base all'abilità dell'Eroe e alla quantità di tokens LP depositati nel Giardino che stanno curando, quindi i giocatori che depositano tokens LP nei Giardini e fanno le missioni in quegli stessi giardini hanno subito un'utilità sinergica per i loro NFT.

Ogni Power Token ha un proprio programma di emissioni. In generale, le emissioni al minuto sono più elevate al momento del lancio del token e diminuiscono nel tempo. Questa diminuzione delle emissioni non è lineare, quindi è importante esaminare i programmi di emissione di ciascun token nella relativa sottopagina de[ I Giardini](./).

Le emissioni sono regolate da periodi di tempo chiamati Epoche. Ogni token inizia nell'Epoca 1 al momento del lancio, che ha il tasso di emissione più alto. Con ogni Epoca, il tasso può cambiare o rimanere costante, come mostrato nella tabella di ogni token nella loro sottopagina dei Gardens.

Le epoche si basano sui timestamp e durano esattamente una settimana.

### Allocazioni e ricompense

La quantità totale di ogni Power Token emesso al minuto può essere determinata dall'Epoca, ma quei tokens devono andare da qualche parte! A ogni singolo Giardino (che rappresenta una specifica coppia di LP incentivati) viene assegnata una quota del totale dei tokens coniati. L'assegnazione per ogni pool incentivata può essere visualizzata nella Seed Box di ogni Regno. In base all'Epoca corrente, al suo tasso di emissione e all'allocazione per una specifica pool, i giocatori possono determinare quanti tokens saranno emessi in quella pool ogni secondo, minuto o giorno. Da qui, la pool divide i tokens tra tutti i giocatori che hanno depositato tokens LP in quella pool in proporzione alla loro quota totale di quella pool e li distribuisce come ricompensa. Quando si effettuano questi calcoli, è indispensabile ricordare che i giocatori possono entrare o uscire liberamente dalle pool di liquidità, per cui la quota di ciascun giocatore è costantemente in movimento, in quanto la liquidità viene aggiunta o rimossa.

#### Allocationi del Progetto

Per finanziare il progetto e sostenere le ricompense per i giocatori, e per evitare di trasferire costi aggiuntivi, ogni volta che un giocatore reclama le proprie ricompense nei Giardini, il contratto MasterGardener conia una percentuale aggiuntiva (dettagliata nelle informazioni sull'allocazione di ciascun token) del token richiesto ai portafogli del progetto, compreso il Jeweler. Queste allocazioni non escono dalle emissioni del Giardino per ogni epoca, come specificato nella pagina dei Giardini di ogni regno, ma contano per la fornitura totale del token. Questi fondi sono soggetti a tassi di blocco separati, come segue:

* Development Fund, Marketing Fund, Jeweler - 45% locked
* Founders Fund - 95% locked

Questi tassi di blocco consentono la stabilità e lo sviluppo del progetto nel tempo, continuando a incentivarne la crescita ed il successo a lungo termine. Inoltre, forniscono ricompense garantite per un lungo periodo di tempo ai giocatori che [depositano sul Jeweler](../il-jeweler/) in ogni regno.

### Modello di Locking ( Blocco )

Per bilanciare gli elevati tassi di emissioni nelle epoche precedenti e per fornire stabilità dei prezzi, la nostra tokenomic include un modello di blocco sui premi dei Gardens. Fino a un certo punto in ogni programma di emissione, viene sbloccata solo una parte dei gettoni farmati, raccolti e distribuiti come ricompense dei giardini agli staker di tokens LP. Una volta richiesti, questi tokens premio sbloccati vengono trasferiti direttamente nel portafoglio del giocatore e sono immediatamente utilizzabili. Tuttavia, anche una parte delle ricompense dei Gardens è bloccata. Questi premi vengono assegnati al portafoglio del giocatore, ma non è possibile accedervi o utilizzarli in alcun modo fino a quando non vengono sbloccati.

Per ogni token, a partire dall'Epoca 1, il 5% delle ricompense richieste viene sbloccato mentre il 95% è bloccato. Ogni Epoca, la percentuale di ricompense che vengono sbloccate aumenta del 2%, quindi nella Epoca 2, il 7% è sbloccato e il 93% è bloccato, e così via. È importante notare che queste percentuali si basano sull'Epoca nel momento in cui il giocatore sceglie di ritirare le ricompense, non quando sono state assegnate. Se un giocatore sceglie di non prelevarle subito, la percentuale che potrà ritirare aumenta del 2% ogni Epoca. Una volta che un giocatore ha prelevato, il resto delle ricompense bloccate smette di essere sbloccato fino all'Epoca 51, a quel punto iniziano a sbloccarsi linearmente nelle 52 Epoche successive. Dopo l'Epoca 51, non si verificheranno ulteriori blocchi e tutte le ricompense appena generate verranno completamente sbloccate subito.

Per ogni token, a partire dall'Epoca 1, il 5% delle ricompense richieste viene sbloccato mentre il 95% viene bloccato. Ogni Epoca, la percentuale di ricompense che vengono sbloccate aumenta del 2%, quindi in Epoca 2, il 7% è sbloccato e il 93% è bloccato, e così via. È importante notare che queste percentuali si basano sull'Epoca nel momento in cui il giocatore sceglie di ritirare i premi e non quando sono state assegnate le ricompense. Se un giocatore sceglie di non rivendicare subito, la percentuale di tokens che verranno sbloccati che potranno richiedere aumenta del 2% ogni Epoca. Una volta che un giocatore ha rivendicato, tuttavia, il resto delle ricompense rivendicate che sono bloccate, rimangono bloccate fino alla fine dell'Epoca 51, a quel punto iniziano a sbloccarsi in modo lineare nelle 52 Epoche successive, a meno che non vengano sbloccate con altri mezzi, come le [Missioni di Mining](../../learn/gameplay/professions/jewel-mining.md). Dopo l'Epoca 51, non si verificheranno ulteriori blocchi e tutte le ricompense generate verranno completamente sbloccate immediatamente.

### Modello di Locking  - Sblocco anticipato con gli Eroi NFT

Una delle caratteristiche più uniche di DeFi Kingdoms sono i nostri Eroi NFT che forniscono una vera utilità in-game. La professione Mining è uno di questi casi d'uso. I giocatori che hanno ricompense bloccate possono inviare i loro Eroi in missioni di JEWEL Mining per sbloccare alcuni di quei tokens in anticipo, garantendo l'accesso alle ricompense bloccate prima del loro sblocco naturale.

Non tutti gli Eroi avranno lo stesso livello di competenza nel Mining, quindi è importante conoscere le varie statistiche utilizzate dagli Eroi e come funziona ogni Professione quando si cerca di acquistarle e usarle. Puoi trovare maggiori dettagli a riguardo nella sezione [Profession Quest](../../learn/gameplay/professions/) dei documenti.

### Commissioni di deposito e prelievo dei Gardens

**Non ci sono commissioni di deposito per lo staking di gettoni LP nei Giardini**. Per proteggerci da prestiti flash e pump and dump, abbiamo implementato commissioni di prelievo per il ritiro dei token LP in staking. Il primo deposito e ogni prelievo successivo azzera il timer della commissione. Le commissioni di prelievo sono elencate di seguito:

* **0.01%** se un utente preleva dopo **4 Epoche**
* **0.25%** se un utente preleva dopo  **2 Epoche ma prima di 4 Epoche**
* **0.5%** se un utente preleva dopo **5 giorni ma prima di 2 Epoche**
* **1%** se un utente preleva prima di **5 giorni. \***
* **2%** se un utente preleva prima di **3 giorni. \***
* **4%** se un utente preleva prima di **24 ore. \***
* **8%** se un utente preleva prima di **1 ora. \***
* **25%** se un utente preleva **durante lo stesso blocco.**

##
