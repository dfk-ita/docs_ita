---
description: Dettagli sul Sistema di Combattimento degli Eroi in DeFi Kingdoms
cover: ../.gitbook/assets/archer_volley.gif
coverY: 0
---

# Combat

Questa pagina contiene informazioni dettagliate sul Sistema di Combattimento degli Eroi di DeFi Kingdoms, che sarà utilizzato nei combattimenti giocatore-vs-giocatore (PVP) e giocatore-vs-ambiente (PVE).

{% hint style="warning" %}
Tutte le informazioni contenute in questa pagina sono considerate "Pre-Alpha" e preliminari e sono pertanto soggette a modifiche. Ultimo aggiornamento: 25/12/2022
{% endhint %}

## Parole Chiave nei Combattimenti <a href="#e28e" id="e28e"></a>

Le **Parole Chiave** hanno un significato ed un impatto specifico sul combattimento. Definiscono varie porzioni di azioni che possono essere intraprese e gli effetti delle **Abilità**. La Parola Chiave stessa è usata come abbreviazione per riferirsi alla sua definizione.

| PAROLA CHIAVE        | DEFINIZIONE                                                                                                                                                                                                                                     |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Action               | Un Attacco Base, l'uso di un Potere, l'uso di un Tratto, l'uso di un Oggetto o il Riposizionamento.                                                                                                                                             |
| AOE                  | Infligge danni ai nemici in Posizione 1, Posizione 2 e Posizione 3. (Danno ad Area)                                                                                                                                                             |
| Backfire             | Se il bersaglio ha ricevuto danni magici, attenua l'X% di tali danni. La fonte del danno riceve un danno pari al valore attenuato.                                                                                                              |
| Banish               | Il bersaglio viene rimosso dal campo di battaglia. Il bersaglio non può attaccare o lanciare un’abilità. Né le abilità né gli attacchi base degli alleati e dei nemici possono colpire questo bersaglio. Interrompe.                            |
| Battle               | Un'istanza PVP/PVE completa.                                                                                                                                                                                                                    |
| Berserk              | Questo Eroe non può essere controllato per 1 Round e lancia un'abilità casuale che ha come bersaglio un nemico o un alleato a caso. Non è possibile puntare su se stessi.                                                                       |
| Bleed                | Danno fisico che persiste per altri Round.                                                                                                                                                                                                      |
| Blind                | La precisione dell'Eroe è ridotta del 50%. Questo effetto di stato persiste finché non viene rimosso.                                                                                                                                           |
| Block                | Annulla i danni in arrivo da un colpo. Se un attacco ha ottenuto un risultato di Colpire tramite un controllo di Precisione, l'istanza di Blocco riduce il danno allo 0%.                                                                       |
| Burn                 | Danno magico che persiste per altri Round dopo l'istanza di danno iniziale.                                                                                                                                                                     |
| Channel              | Un Eroe lancia un incantesimo così potente da richiedere un intero turno (o più) di carica prima di lanciare l'incantesimo.                                                                                                                     |
| Cleanse              | Rimuove tutti gli effetti di stato negativi dal bersaglio.                                                                                                                                                                                      |
| Cleave               | Infligge danni ai nemici in Posizione 1 e Posizione 2.                                                                                                                                                                                          |
| Combo                | Se si ottiene un'azione prerequisita, al lancio di un'abilità con COMBO può avere luogo un buff o un'azione speciale.                                                                                                                           |
| Confused             | Le abilità del bersaglio hanno una probabilità del 50% di colpire un bersaglio alternativo casuale, compreso il bersaglio personale. Interrompe.                                                                                                |
| Daze                 | Il prossimo turno del bersaglio viene spostato come ultimo del round. Interrompe                                                                                                                                                                |
| Degree of Difficulty | Un'Abilità così complessa che la sua difficoltà comporta una diminuzione della Precisione.                                                                                                                                                      |
| Disarm               | Il bersaglio non può effettuare un Attacco Base o lanciare un Potere in questo Round. Interrompe.                                                                                                                                               |
| Ethereal             | Il bersaglio non può essere spostato, può lanciare solo Abilità magiche e riceve solo danni magici.                                                                                                                                             |
| Execute              | Quando un bersaglio ha meno dell'X% dei suoi HP rimanenti, lo uccide.                                                                                                                                                                           |
| Exhausted            | L'Eroe non può compiere un'Azione nel prossimo turno (per 1 Round). Interrompe.                                                                                                                                                                 |
| Evasion              | L'EVA crea una possibilità per il bersaglio di evitare un attacco in arrivo, sia esso magico o fisico. Un'EVA del 50% riduce del 50% la Precisione di un attacco in arrivo.                                                                     |
| Fear                 | Se un bersaglio è sotto lo stato Fear, il bersaglio è Push 1. Il bersaglio non può eseguire alcuna Azione che infligga danni fisici per 2 Round. Interrompe.                                                                                    |
| First Strike         | Il bersaglio agisce per primo il prossimo Round. Se più bersagli hanno First Strike, il bersaglio con l'AGI più alta agisce per primo.                                                                                                          |
| Interrupt            | Un'abilità che impedisce ad un bersaglio di Incanalare un potere ed azzera il costo del potere e del mana.                                                                                                                                      |
| Item                 | Un oggetto fisico non arma utilizzabile in battaglia. Si conserva nell'inventario come le pozioni e le tinture.                                                                                                                                 |
| Lifesteal            | Ogni attacco base o danno abilità restituisce l'X% dei danni inflitti come HP.                                                                                                                                                                  |
| Mana Burn            | I danni inflitti al bersaglio riducono il Mana del bersaglio.                                                                                                                                                                                   |
| Pierce               | Se il bersaglio ha una resistenza ai danni, infligge danni come se quella resistenza fosse inferiore dell'X%, dove X = la Penetrazione dell'abilità.                                                                                            |
| Poison               | Danno fisico che si accelera nel tempo. Infligge danni pari al 2% degli HP massimi dell'Eroe all'inizio di ogni Round. Ogni Round in cui persiste, impila un ulteriore 2% di danni agli HP massimi. Limitato al 20% degli HP massimi per turno. |
| Pull                 | Un'abilità che sposta il bersaglio di 1 posizione in avanti. Interrompe.                                                                                                                                                                        |
| Push                 | Un'abilità che sposta il bersaglio di 1 posizione indietro. Interrompe.                                                                                                                                                                         |
| Reposition           | Un Eroe può spendere il proprio turno spostandosi in una posizione diversa che si trova ad una (1) posizione di distanza: P1 a P2, P2 a P3, P3 a P2, ecc.                                                                                       |
| Riposte              | Se il bersaglio ha ricevuto danni fisici, attenua l'X% di tali danni. La fonte del danno riceve un danno pari al valore attenuato.                                                                                                              |
| Round                | Iniziando con 1 Eroe, ruota completamente attraverso tutti i turni degli Eroi fino a quando non ritorna il turno dell'Eroe di partenza.                                                                                                         |
| Sanjo Hair           | Il mostro bersaglio con Sanjo Hair non può subire Push, Pull, Daze o Stun.                                                                                                                                                                      |
| Silence              | Se un Eroe è silenziato, non può infliggere danni magici, guarire o lanciare un'abilità magica per 2 Round. Interrompe.                                                                                                                         |
| Sleep                | Il nemico bersaglio non può compiere azioni finché non viene bersagliato da un'abilità di un nemico o di un alleato. Interrompe.                                                                                                                |
| Slow                 | Riduce l'AGI del bersaglio. Un rallentamento del 50% fa sì che un Eroe con 10 AGI funzioni con un'AGI effettiva di 5 in combattimento.                                                                                                          |
| Stacks               | Un valore che può incrementare (impilarsi). Ad esempio, un'abilità che aggiunge l'1% di danni su 3 istanze, aggiunge il 3% di danni.                                                                                                            |
| Status Effect        | Qualsiasi abilità duratura che potenzia o indebolisce un bersaglio.                                                                                                                                                                             |
| Stun                 | Il turno successivo del bersaglio viene saltato (1 Round). Interrompe.                                                                                                                                                                          |
| Turn                 | 1 Azione Eroe. 1 Turno è terminato dopo che tutti i partecipanti hanno effettuato 1 Turno.                                                                                                                                                      |
| Unstoppable          | Non può essere influenzato da effetti di stato negativi.                                                                                                                                                                                        |
| Untargetable         | Né le abilità né gli attacchi base degli alleati e dei nemici possono colpire questo Eroe.                                                                                                                                                      |

## Tratti Genetici <a href="#08a5" id="08a5"></a>

Tutti gli Eroi hanno **Tratti Genetici**, alcuni dei quali sono **Attivi** ed altri **Passivi**, tutti suddivisi in livelli base, avanzati, d’élite ed exalted.

### Tratti Genetici Attivi <a href="#1e88" id="1e88"></a>

I Tratti Attivi di un Eroe possono essere attivati una volta per battaglia ed utilizzano un’Azione. Non hanno un costo di Mana.

| TRATTO      | NOME            | FUNZIONE                                                                                                                                                     |
| ----------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Basic 1     | Poisoned Blade  | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Questo attacco ha una probabilità dell'80% di avvelenare il nemico bersaglio.                        |
| Basic 2     | Blinding Winds  | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Questo attacco ha una probabilità dell'80% di accecare il nemico bersaglio.                          |
| Basic 3     | Heal            | Cura l'Eroe bersaglio per il 20% degli HP massimi.                                                                                                           |
| Basic 4     | Cleanse         | Rimuove gli Effetti di Stato dall'Eroe bersaglio.                                                                                                            |
| Basic 5     | Iron Skin       | Riduce i danni fisici subiti del 20% per 4 turni.                                                                                                            |
| Basic 6     | Speed           | Guadagna First Strike in ciascuno dei 2 round successivi.                                                                                                    |
| Basic 7     | Critical Aim    | Attivare per ottenere una probabilità aggiuntiva del 70% di Crit per 2 round. Infligge al nemico bersaglio danni pari a (1,0\*Basic).                        |
| Basic 8     | Deathmark       | Il nemico bersaglio riceve il 20% di danni in più dagli alleati per 2 round. Infligge al nemico bersaglio danni pari a (1,0\*Basic).                         |
| <p><br></p> | <p><br></p>     | <p><br></p>                                                                                                                                                  |
| Advanced 1  | Exhaust         | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Applica l’Effetto di stato Exhausted sul bersaglio                                                   |
| Advanced 2  | Daze            | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Applica l’Effetto di stato Dazed sul bersaglio                                                       |
| Advanced 3  | Explosion       | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Questo attacco esplode per il 100% dei danni inflitti in un AOE, infliggendo danni a tutti i nemici. |
| Advanced 4  | Hardened Shield | Riduce i danni fisici subiti del 30% per 4 turni.                                                                                                            |
| <p><br></p> | <p><br></p>     | <p><br></p>                                                                                                                                                  |
| Elitè 1     | Stun            | Infligge al nemico bersaglio danni pari a (1,0\*Basic). Applica l’Effetto di stato Stunned sul bersaglio                                                     |
| Elitè 2     | Second Wind     | L'Eroe si cura per il 50% degli HP mancanti. Tutti i membri del gruppo vengono curati per il 75% di quel valore.                                             |
| <p><br></p> | <p><br></p>     | <p><br></p>                                                                                                                                                  |
| Exalted     | Resurrection    | Riporta in vita un alleato bersaglio. L'alleato bersaglio torna Exhausted e con il 50% di HP massimi.                                                        |

### Tratti Genetici Passivi

I Tratti Passivi di un Eroe vengono applicati quando l’Eroe è presente sul campo di battaglia. Questi Tratti possono essere impilati, ma alcuni hanno dei limiti.

| TRATTO      | NOME         | FUNZIONE                                                                                                                                         |
| ----------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Basic 1     | Duelist      | Quando si combatte 1v1, guadagna il 20% di danni bonus.                                                                                          |
| Basic 2     | Clutch       | Aumenta i danni inflitti del 30% quando la salute è inferiore al 30%.                                                                            |
| Basic 3     | Foresight    | Guadagna permanentemente l'8% di evasione.                                                                                                       |
| Basic 4     | Headstrong   | 40% di probabilità di non essere influenzato da Daze.                                                                                            |
| Basic 5     | Clear Vision | 40% di probabilità di non essere influenzato da Blind.                                                                                           |
| Basic 6     | Fearless     | 40% di probabilità di non essere influenzato da Fear.                                                                                            |
| Basic 7     | Chatterbox   | 40% di probabilità di non essere influenzato da Silence.                                                                                         |
| Basic 8     | Stalwart     | 40% di probabilità di non essere influenzato da Poison.                                                                                          |
| <p><br></p> | <p><br></p>  | <p><br></p>                                                                                                                                      |
| Advanced 1  | Leadership   | Gli alleati infliggono il 5% di danni bonus. Questo bonus non può superare il 15% totale di squadra.                                             |
| Advanced 2  | Efficent     | Riduce il consumo di mana del 10%.                                                                                                               |
| Advanced 3  | Intimidation | I nemici infliggono il 5% di danni in meno. Questo bonus non può superare il 15% totale di squadra.                                              |
| Advanced 4  | Toxic        | Ogni volta che questo Eroe subisce danni ha una probabilità del 2% di applicare avvelenamento.                                                   |
| <p><br></p> | <p><br></p>  | <p><br></p>                                                                                                                                      |
| Elitè 1     | Giant Slayer | Se il nemico bersaglio possiede attualmente più HP di questo Eroe, infligge il 30% di danni bonus agli Eroi e il 10% di danni bonus ai Mostri.   |
| Elitè 2     | Last Stand   | Quando la salute di questo Eroe scende sotto il 20%, diventa Invulnerabile per 1 Round. Può verificarsi solo una volta per battaglia e per gene. |
| <p><br></p> | <p><br></p>  | <p><br></p>                                                                                                                                      |
| Exalted     | Second Life  | Alla morte, riporta in vita questo Eroe esausto e con il 50% di HP massimi. Può verificarsi solo una volta per battaglia e per gene.             |

\
