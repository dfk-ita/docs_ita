# Giardini JEWEL

### **Programma di emissione**

L'emissione di JEWEL come ricompensa per lo staking di token LP nel Garden è programmata per cambiare durante ogni periodo di tempo consecutivo, che chiamiamo Epoca. Ogni Epoca è di 302,400 blocchi su Harmony Blockchain e la lunghezza di ogni Epoca dipende dalla velocità media dei blocchi su Harmony. Le Epoche sono state calcolate a 302.400 blocchi in modo che ogni Epoca equivalga a una settimana assumendo una velocità di 2 secondi per blocco su Harmony Blockchain. Tuttavia, se le velocità dei blocchi sono in media più lunghe di 2 secondi per blocco, un'Epoca durerà più di una settimana .

| Epoca | Blocco     | JEWEL/blocco | JEWEL/minuto |
| ----- | ---------- | ------------ | ------------ |
| 1     | 16,350,367 | 256          | 7680         |
| 2     | 16,652,767 | 128          | 3840         |
| 3     | 16,955,167 | 96           | 2880         |
| 4     | 17,257,567 | 64           | 1920         |
| 5     | 17,559,967 | 56           | 1680         |
| 6     | 17,862,367 | 48           | 1440         |
| 7     | 18,164,767 | 40           | 1200         |
| 8     | 18,467,167 | 32           | 960          |
| 9     | 18,769,567 | 28           | 840          |
| 10    | 19,071,967 | 24           | 720          |
| 11    | 19,374,367 | 20           | 600          |
| 12    | 19,676,767 | 16           | 480          |
| 13    | 19,979,167 | 15           | 450          |
| 14    | 20,281,567 | 14           | 420          |
| 15    | 20,583,967 | 13           | 390          |
| 16    | 20,886,367 | 12           | 360          |
| 17    | 21,188,767 | 11           | 330          |
| 18    | 21,491,167 | 10           | 300          |
| 19    | 21,793,567 | 9            | 270          |
| 20-35 | 22,095,967 | 8            | 240          |
| 36+   | 26,934,367 | 4            | 120          |

_\*I moltiplicatori elencati sono distribuiti in tutti i giardini. Puoi vedere il Seed Box per i tassi di emissione specifici per ogni pool._

Visita [Harmony Blockchain Explorer](https://explorer.harmony.one/) per vedere qual è il blocco corrente e la velocità del blocco corrente (latenza). Tieni presente che la velocità di blocco varia e dovrebbe essere visualizzata in media (ovvero su base giornaliera o settimanale) quando provi a pianificare le strategie di farming del tuo giardino.

### Locking

I JEWEL bloccati prelevati  rimarranno  **bloccati fino al blocco 31,470,366**, che segna la fine dell'Epoca 51. Le ricompense bloccate inizieranno a sbloccarsi linearmente nelle 52 Epoche successive. Attualmente, si stima che lo sblocco inizi nel terzo trimestre del 2022; tuttavia, la latenza di rete ha già esteso la durata della maggior parte delle epoche e non è possibile determinare una data specifica in cui verrà raggiunto questo specifico blocco di Harmony.&#x20;

La percentuale di JEWEL sbloccati inizia al 5% in Epoch 1 e aumenta del 2% in ogni Epoca. Le ricompense non riscosse continuano a essere sbloccate in questo modo fino al loro prelievo, momento in cui le ricompense sbloccate vanno direttamente nel portafoglio del giocatore e le ricompense bloccate diventano completamente bloccate fino alla fine dell'Epoca 51.

### Modello di Locking - Esempi semplificati

Di seguito sono riportati due esempi semplificati che mostrano come funziona il modello di blocco. Per semplicità, **gli esempi presuppongono che non vengano reinvestite le ricompense sbloccate** in posizioni LP aggiuntive e che un giocatore abbia guadagnato 100 JEWEL in ricompense dai Giardini durante l'Epoca 1, 50 JEWEL nell'Epoca 2 e così via per riflettere la ridotta emissione di JEWEL per Epoca. In entrambi gli scenari, si guadagnano 301,6 JEWEL, ma l'importo sbloccato rispetto a quello bloccato è diverso. Questo modello di blocco offre ai giocatori l'opportunità di scegliere una strategia adatta al loro stile e alla loro propensione al rischio.&#x20;

**Esempio illustrativo A**: I premi guadagnati durante ogni Epoca vengono prelevati durante ogni Epoca (e non reinvestiti).

*   Riassunto di 10 Epoche:

    * Totale JEWEL sbloccati: **29.8** JEWEL
    * Totale JEWEL bloccati: **271.8** JEWEL ( inaccessibili fino a dopo l'Epoca 51 a meno che non siano sbloccati in anticipo tramite gli Eroi)
    * Ricompense totali: **301.6** JEWEL
    * _Riduce i JEWEL sbloccati durante il periodo in esame, ma consente l'uso e il potenziale reinvestimento dei JEWEL sbloccati, il che potrebbe comportare più JEWEL sbloccati rispetto al mancata prelievo nello stesso periodo. A voi la scelta!_



| Epoca | Sbloccati al prelievo | Bloccati al prelievo | JEWEL guadagnati per Epoca nell'Esempio A | Jewel sbloccati prelevati per Epoca | JEWEL sbloccati cumulativi | JEWEL bloccati cumulativi |
| ----- | --------------------- | -------------------- | ----------------------------------------- | ----------------------------------- | -------------------------- | ------------------------- |
| 1     | 5%                    | 95%                  | 100.0                                     | 5.0                                 | 5.0                        | 95.0                      |
| 2     | 7%                    | 93%                  | 50.0                                      | 3.5                                 | 8.5                        | 141.5                     |
| 3     | 9%                    | 91%                  | 37.5                                      | 3.4                                 | 11.9                       | 175.6                     |
| 4     | 11%                   | 89%                  | 25.0                                      | 2.8                                 | 14.6                       | 197.9                     |
| 5     | 13%                   | 87%                  | 21.9                                      | 2.8                                 | 17.5                       | 216.9                     |
| 6     | 15%                   | 85%                  | 18.8                                      | 2.8                                 | 20.3                       | 232.8                     |
| 7     | 17%                   | 83%                  | 15.6                                      | 2.7                                 | 22.9                       | 245.8                     |
| 8     | 19%                   | 81%                  | 12.5                                      | 2.4                                 | 25.3                       | 255.9                     |
| 9     | 21%                   | 79%                  | 10.9                                      | 2.3                                 | 27.6                       | 264.6                     |
| 10    | 23%                   | 77%                  | 9.4                                       | 2.2                                 | 29.8                       | 271.8                     |

**Esempio Illustrativo B**: Le ricompense non sono prelevate fino alla fine dell'Epoca 10.

* Riassunto di 10 Epoche:
  * Totale JEWEL sbloccati: **69.4** JEWEL
  * Totale JEWEL bloccati: **232.2** JEWEL ( inaccessibili fino a dopo l'Epoca 51 a meno che non siano sbloccati in anticipo tramite gli Eroi)
  * Ricompense totali: **301.6** JEWEL
  * _Numero di JEWEL sbloccati più alto entro la fine del periodo in esame, ma non è possibile utilizzare o reinvestire i JEWEL sbloccati durante il periodo._

| Epoca | Sbloccati al prelievo | Bloccati al prelievo | JEWEL guadagnati per Epoca nell'Esempio A | Jewel sbloccati cumulativi | JEWEL sbloccati e non prelevati cumulativi | JEWEL bloccati e non prelevati cumulativi | JEWEL sbloccati e prelevati cumulativi | JEWEL bloccati e prelevati cumulativi |
| ----- | --------------------- | -------------------- | ----------------------------------------- | -------------------------- | ------------------------------------------ | ----------------------------------------- | -------------------------------------- | ------------------------------------- |
| 1     | 5%                    | 95%                  | 100.0                                     | 5.0                        | 5.0                                        | 95.0                                      | 0.0                                    | 0.0                                   |
| 2     | 7%                    | 93%                  | 50.0                                      | 3.5                        | 10.5                                       | 139.5                                     | 0.0                                    | 0.0                                   |
| 3     | 9%                    | 91%                  | 37.5                                      | 3.4                        | 16.9                                       | 170.6                                     | 0.0                                    | 0.0                                   |
| 4     | 11%                   | 89%                  | 25.0                                      | 2.8                        | 23.4                                       | 189.1                                     | 0.0                                    | 0.0                                   |
| 5     | 13%                   | 87%                  | 21.9                                      | 2.8                        | 30.5                                       | 203.9                                     | 0.0                                    | 0.0                                   |
| 6     | 15%                   | 85%                  | 18.8                                      | 2.8                        | 38.0                                       | 215.2                                     | 0.0                                    | 0.0                                   |
| 7     | 17%                   | 83%                  | 15.6                                      | 2.7                        | 45.7                                       | 223.1                                     | 0.0                                    | 0.0                                   |
| 8     | 19%                   | 81%                  | 12.5                                      | 2.4                        | 53.4                                       | 227.8                                     | 0.0                                    | 0.0                                   |
| 9     | 21%                   | 79%                  | 10.9                                      | 2.3                        | 61.4                                       | 230.8                                     | 0.0                                    | 0.0                                   |
| 10    | 23%                   | 77%                  | 9.4                                       | 2.2                        | 69.4                                       | 232.2                                     | 69.4                                   | 232.2                                 |

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

_\*I giorni e le ore elencati presuppongono una velocità di blocco di 2 secondi durante tale periodo e dipenderanno dalla velocità della blockchain di Harmony_.\
