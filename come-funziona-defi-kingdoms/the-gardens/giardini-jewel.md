# Giardini JEWEL

{% hint style="danger" %}
In conformità con il [voto governance della Community](https://vote.defikingdoms.com/#/proposal/0x2a83ec79bf88a5d8170b831b4c941a934e47ca0c569a40bb8d240666978b73e6) adottato il 9/1/2022, **le emissioni JEWEL su Harmony sono terminate ed i JEWEL bloccati non si sbloccheranno mai.**\


Per maggiori dettagli su queste modifiche, leggere la [tokenomic aggiornata](../i-token-del-potere/jewel-token.md#tokenomic-aggiornata) del progetto.
{% endhint %}

{% hint style="info" %}
Per quanto sopra, le informazioni riportate di seguito sui Giardini JEWEL su Serendale non sono più applicabili, ma sono state lasciate qui come riferimento.
{% endhint %}

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

I JEWEL bloccati prelevati  rimarranno  **bloccati fino al blocco 31,772,767**, che segna la fine dell'Epoca 51. Le ricompense bloccate inizieranno a sbloccarsi linearmente nelle 52 Epoche successive. Attualmente, si stima che lo sblocco inizi nel terzo trimestre del 2022; tuttavia, la latenza di rete ha già esteso la durata della maggior parte delle epoche e non è possibile determinare una data specifica in cui verrà raggiunto questo specifico blocco di Harmony.&#x20;

La percentuale di JEWEL sbloccati inizia al 5% in Epoch 1 e aumenta del 2% in ogni Epoca. Le ricompense non riscosse continuano a essere sbloccate in questo modo fino al loro prelievo, momento in cui le ricompense sbloccate vanno direttamente nel portafoglio del giocatore e le ricompense bloccate diventano completamente bloccate fino alla fine dell'Epoca 51.

### Modello di Locking - Esempi semplificati

Di seguito sono riportati due esempi semplificati che mostrano come funziona il modello di blocco. Per semplicità, **gli esempi presuppongono che non venga fatto il compound delle ricompense sbloccate** in posizioni LP aggiuntive e che un giocatore abbia guadagnato 100 JEWEL in ricompense dai Giardini durante l'Epoca 1, 50 JEWEL nell'Epoca 2 e così via per riflettere la ridotta emissione di JEWEL per Epoca. In entrambi gli scenari, si guadagnano 301,6 JEWEL, ma l'importo sbloccato rispetto a quello bloccato è diverso. Questo modello di blocco offre ai giocatori l'opportunità di scegliere una strategia adatta al loro stile e alla loro propensione al rischio.&#x20;

**Esempio illustrativo A**: I premi guadagnati durante ogni Epoca vengono prelevati durante ogni Epoca (e non utilizzati in compound).

*   Riassunto di 10 Epoche:

    * Totale JEWEL sbloccati: **29.8** JEWEL
    * Totale JEWEL bloccati: **271.8** JEWEL ( inaccessibili fino a dopo l'Epoca 51 a meno che non siano sbloccati in anticipo tramite gli Eroi)
    * Ricompense totali: **301.6** JEWEL
    * _Riduce i JEWEL sbloccati durante il periodo in esame, ma consente l'uso e il potenziale compound dei JEWEL sbloccati, il che potrebbe comportare più JEWEL sbloccati rispetto al mancata prelievo nello stesso periodo. A voi la scelta!_



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

<table><thead><tr><th>Epoca</th><th>Sbloccati al prelievo</th><th>Bloccati al prelievo</th><th>JEWEL guadagnati per Epoca nell'Esempio A</th><th>Jewel sbloccati cumulativi</th><th width="239">JEWEL sbloccati e non prelevati cumulativi</th><th>JEWEL bloccati e non prelevati cumulativi</th><th>JEWEL sbloccati e prelevati cumulativi</th><th>JEWEL bloccati e prelevati cumulativi</th></tr></thead><tbody><tr><td>1<br></td><td>5%</td><td>95%</td><td>100.0</td><td>5.0</td><td>5.0</td><td>95.0</td><td>0.0</td><td>0.0</td></tr><tr><td>2</td><td>7%</td><td>93%</td><td>50.0</td><td>3.5</td><td>10.5</td><td>139.5</td><td>0.0</td><td>0.0</td></tr><tr><td>3</td><td>9%</td><td>91%</td><td>37.5</td><td>3.4</td><td>16.9</td><td>170.6</td><td>0.0</td><td>0.0</td></tr><tr><td>4</td><td>11%</td><td>89%</td><td>25.0</td><td>2.8</td><td>23.4</td><td>189.1</td><td>0.0</td><td>0.0</td></tr><tr><td>5</td><td>13%</td><td>87%</td><td>21.9</td><td>2.8</td><td>30.5</td><td>203.9</td><td>0.0</td><td>0.0</td></tr><tr><td>6</td><td>15%</td><td>85%</td><td>18.8</td><td>2.8</td><td>38.0</td><td>215.2</td><td>0.0</td><td>0.0</td></tr><tr><td>7</td><td>17%</td><td>83%</td><td>15.6</td><td>2.7</td><td>45.7</td><td>223.1</td><td>0.0</td><td>0.0</td></tr><tr><td>8</td><td>19%</td><td>81%</td><td>12.5</td><td>2.4</td><td>53.4</td><td>227.8</td><td>0.0</td><td>0.0</td></tr><tr><td>9</td><td>21%</td><td>79%</td><td>10.9</td><td>2.3</td><td>61.4</td><td>230.8</td><td>0.0</td><td>0.0</td></tr><tr><td>10</td><td>23%</td><td>77%</td><td>9.4</td><td>2.2</td><td>69.4</td><td>232.2</td><td>69.4</td><td>232.2</td></tr></tbody></table>
