# Ice Gardens

### **Programma di emissione**

L'emissione di CRYSTAL è programmata per cambiare durante ogni periodo di tempo consecutivo, che chiamiamo Epoca. Ogni Epoca dura esattamente una settimana e inizia alle 20:00 EST della data elencata nella tabella seguente:

| Epoca  | Blocco           | CRYSTAL/blocco | CRYSTAL/minuto |
| ------ | ---------------- | -------------- | -------------- |
| 1      | 30 Marzo 2022    | 32             | 960            |
| 2      | 6 Aprile 2022    | 24             | 720            |
| 3      | 13 Aprile 2022   | 20             | 600            |
| 4      | 20 Aprile 2022   | 16             | 480            |
| 5      | 27 Aprile 2022   | 14             | 420            |
| 6      | 4 Maggio 2022    | 12             | 360            |
| 7      | 11 Maggio 2022   | 10             | 300            |
| 8      | 18 Maggio 2022   | 10             | 300            |
| 9      | 25 Maggio 2022   | 8              | 240            |
| 10     | 1 Giugno 2022    | 8              | 240            |
| 11     | 8 Giugno 2022    | 6              | 180            |
| 13     | 15 Giugno 2022   | 6              | 180            |
| 13     | 22 Giugno 2022   | 4              | 120            |
| 14     | 29 Giugno 2022   | 4              | 120            |
| 15     | 6 Luglio 2022    | 4              | 120            |
| 16     | 13 Luglio 2022   | 4              | 120            |
| 17     | 20 Luglio 2022   | 3              | 90             |
| 18     | 27 Luglio 2022   | 3              | 90             |
| 19     | 3 Agosto 2022    | 3              | 90             |
| 20     | 10 Agosto 2022   | 3              | 90             |
| 21-100 | 17 Agosto 2022   | 2              | 60             |
| 101+   | 28 Febbraio 2024 | 1              | 30             |

### Locking

I CRYSTAL bloccati prelevati  rimarranno  **bloccati fino al 22 Marzo 2023,\*\*,\*\*** che segna la fine dell'Epoca 51. Le ricompense bloccate inizieranno a sbloccarsi linearmente nelle 52 Epoche successive. &#x20;

La percentuale di CRYSTAL sbloccati inizia al 5% in Epoch 1 e aumenta del 2% in ogni Epoca. Le ricompense non riscosse continuano a essere sbloccate in questo modo fino al loro prelievo, momento in cui le ricompense sbloccate vanno direttamente nel portafoglio del giocatore e le ricompense bloccate diventano completamente bloccate fino alla fine dell'Epoca 51.

### Commissioni di deposito e prelievo dei Gardens

**Non ci sono commissioni di deposito per lo staking di token LP nei Giardini**. Per proteggerci da prestiti flash e pump and dump, abbiamo implementato commissioni di prelievo per il ritiro di token LP in staking. Ogni prelievo azzera il timer della commissione. Le commissioni di prelievo sono elencate di seguito:

* **0.01%** se un utente preleva dopo **4 Epoche**
* **0.25%** se un utente preleva dopo  **2 Epoche ma prima di 4 Epoche**
* **0.5%** se un utente preleva dopo **5 giorni ma prima di 2 Epoche**
* **1%** se un utente preleva prima di **5 giorni.**&#x20;
* **2%** se un utente preleva prima di **3 giorni.**&#x20;
* **4%** se un utente preleva prima di **24 ore.**&#x20;
* **8%** se un utente preleva prima di **1 ora.**&#x20;
* **25%** se un utente preleva **durante lo stesso blocco.**

__
