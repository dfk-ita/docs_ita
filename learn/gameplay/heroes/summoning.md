# Summoning

<figure><img src="../../../.gitbook/assets/image.png" alt="" width="563"><figcaption><p>Il Portale di Evocazione di Crystalvale</p></figcaption></figure>

Per evocare, due Eroi devono recarsi dall'**Arcidruido** ed infondere un Cristallo dell'Evocazione con la loro essenza combinata. I **Cristalli Infusi** vengono poi utilizzati nel [Portale](../../../gameplay/zone-di-gioco/portal.md) per cercare Eroi da terre lontane che siano in sintonia con gli Eroi che hanno infuso il cristallo.

![Infused Crystal](https://dfk-hv.b-cdn.net/art-assets/crystal-yellow.gif)

Per infondere un cristallo, gli Eroi versano la loro energia nelle **Gaia's Tears** e nel **Power Token** di quel regno, che vengono poi immessi in un Cristallo di Evocazione. Gli Eroi più forti possono usare altre Gaia's Tears per far sì che il portale cerchi Eroi più forti e più simili all'evocatore.

{% hint style="info" %}
Nota: gli Eroi evocati sono troppo simili agli Eroi che li hanno evocati per poter sintonizzare correttamente un nuovo Cristallo di Evocazione. Questo vale anche per le coppie di Eroi che sono state evocate da uno o due degli stessi Eroi. Tutte le altre combinazioni di Eroi non avranno problemi a sintonizzare un Cristallo di Evocazione, purché abbiano ancora energia di sintonizzazione.
{% endhint %}

Per ogni 5 livelli raggiunti da un Eroe evocatore, questi può aumentare il costo delle Gaia's Tears di 10 per fornire bonus all'Eroe evocato. Tali bonus vengono applicati alle statistiche dell'Eroe evocato, alla crescita primaria delle statistiche e alla crescita secondaria delle statistiche. I bonus si basano sulle prime tre statistiche dell'Eroe evocato e ogni Eroe evocato può fornire i propri bonus se usa lacrime extra.

I bonus seguono il seguente schema, con ogni incremento di +10 Tears per ogni Eroe evocatore:

1. \+(1 + loopCount) per corrispondere alle statistiche più alte dell'Eroe evocatore
2. \+(1 + loopCount)% al tasso di crescita delle statistiche primarie della statistica più alta dell'Eroe evocatore
3. \+(2 + loopCount)% al tasso di crescita delle statistiche secondarie della statistica più alta dell'Eroe evocatore
4. \+(1 + loopCount) per stat corrispondente alla seconda statistica più alta dell'Eroe evocatore
5. \+(1 + loopCount)% al tasso di crescita delle statistiche primarie corrispondente alla seconda statistica più alta dell'Eroe evocatore
6. \+(2 + loopCount)% al tasso di crescita delle statistiche secondarie corrispondente alla seconda statistica più alta dell'Eroe evocatore
7. \+(1 + loopCount) per stat corrispondente alla terza statistica più alta dell'Eroe evocatore
8. \+(1 + loopCount)% al tasso di crescita delle statistiche primarie corrispondente alla terza statistica più alta dell'Eroe evocatore
9. \+(2 + loopCount)% al tasso di crescita delle statistiche secondarie corrispondente alla terza statistica più alta dell'Eroe evocatore

In queste formule, loopCount indica il numero di volte in cui i bonus sono tornati al passaggio 1 (questo accade a +100 e +190 Tears aggiunte). Quindi la seconda volta, al passaggio 1 il bonus aggiunto sarebbe +2 alla statistica più alta dell'Eroe evocatore, e così via.

**Esempi:**\
LVL30 Wizard (statistiche più alte INT, WIS e LCK) paga 70 Gaia's Tears (base 10 + 60 per 6 step di 5 livelli) L'Eroe evocato riceve +1 a INT e WIS, +1% di crescita delle statistiche primarie a INT e WIS e +2% di crescita delle statistiche secondarie a INT e WIS

LVL100 Wizard (statistiche più alte INT, WIS e LCK) paga 210 Gaia's Tears (base 10 + 200 per 20 passaggi di 5 livelli) L'eroe evocato riceve +6 a INT, +3 WIS e +3 LCK, +6% statistica primaria crescita a INT, +3% a WIS e 3% a LCK e +5% di crescita statistica secondaria a INT, WIS e LCK

<figure><img src="../../../.gitbook/assets/image (3).png" alt="" width="223"><figcaption></figcaption></figure>

Questi bonus sono **per** **ogni Eroe evocato**, quindi il massimo che due Eroi di LVL100 possono spendere è di 420 Gaia's Tears (10_2 di base + 200_2 extra).

Le **Enhancement Stones** possono essere utilizzate anche durante questo processo per migliorare ulteriormente i parametri di partenza dell'Eroe evocato!

L'atto dell'Evocazione è un processo estenuante e l'esaurimento aumenta ad ogni atto di Evocazione. Per ogni Evocazione che un Eroe compie, deve attendere un **periodo di cooldown** prima di poter Evocare di nuovo. Il periodo di cooldown = ((heroGen \* 4 ore) + 4 ore) \* summonsUsed. Il periodo di cooldown massimo per gli Eroi Gen0 è di 72 ore. Inoltre, ad eccezione degli Eroi Gen0, tutti i nuovi Eroi evocati hanno un periodo di cooldown di 24 ore prima di poter essere evocati.

L'esaurimento dell'Evocazione non si esaurisce con il solo cooldown. Anche la quantità di Power Tokens necessari ad ogni Eroe per infondere il prossimo Cristallo di Evocazione aumenta di 2 Power Tokens dopo ogni Evocazione. Gli Eroi Gen0 hanno il costo iniziale più basso per l'Evocazione (6 Power Tokens), ed ogni generazione superiore alla 0 vedrà un aumento del costo delle proprie Evocazioni di 10 Power Tokens per generazione rispetto alle generazioni inferiori. L'aumento del costo per l'Evocazione dei Gen0 finirà per raggiungere un prezzo inferiore a quello che le generazioni successive pagheranno per effettuare l'Evocazione finale.

Che cos'è? Sì, purtroppo solo gli Eroi Gen0 sono in grado di mantenere la sintonia con Gaia, Evocazione dopo Evocazione. Tutte le generazioni successive hanno semplicemente un limite al numero di volte in cui possono concentrare le loro energie nelle Gaia's Tears. Una volta esaurite le ultime energie di sintonizzazione, non possono più evocare. Un'altra stranezza del processo di evocazione è che il portale cerca coloro che hanno una forza di sintonizzazione con Gaia simile a quella dell'evocatore più debole. Quindi, se un Eroe Evocatore Gen0 infonde un cristallo con un Eroe Evocatore Gen1 con solo quattro evocazioni rimanenti di sintonia, il Gen2 evocato sarà in grado di evocare solo tre volte (lo stesso numero di evocazioni rimanenti dell'evocatore più debole dopo aver evocato questo nuovo eroe). Due evocatori Gen0 evocheranno un Gen1 con dieci evocazioni di sintonia.

## Gradi degli Eroi

Gli Eroi di grado superiore hanno iniziato ad arrivare nel regno!!!

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

L'evocazione con Eroi che hanno i geni appropriati può provocare una mutazione genetica che porta a evocare un Eroe di grado superiore. La tabella qui sopra mostra le combinazioni genetiche necessarie per Evocare ogni possibile classe di Eroi. Gli Eroi di grado superiore hanno statistiche di partenza e parametri di crescita delle statistiche migliori rispetto a quelli di grado inferiore. Tuttavia, un effetto collaterale delle loro abilità avanzate è che richiedono più Gaia's Tears per effettuare un'Evocazione rispetto agli Eroi di grado inferiore. Inoltre, gli Eroi di grado superiore sono più difficili da localizzare per il Portale, quindi gli Eroi di grado superiore hanno evocazioni massime inferiori rispetto a quelli di grado inferiore. La tabella qui sopra mostra i requisiti delle Gaia's Tears per i gradi più alti ed il numero massimo di evocazioni che le classi di grado superiore possono ricevere durante l'evocazione.

Basic - Warrior, Knight, Thief, Archer, Priest, Wizard, Monk, Pirate, Berserker, Seer, Legionnaire, Scholar

Advanced - Paladin, Dark Knight, Summoner, Ninja, Shapeshifter, Bard

Elite - Dragoon, Sage, Spellbow

Exalted - DreadKnight

## Rarità degli Eroi

Il livello di rarità di un Eroe Evocato è influenzato dalla rarità dei due Eroi utilizzati per infondere il Cristallo di Evocazione.

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

La tabella qui sopra illustra la probabilità che accoppiando Eroi di determinate rarità si ottenga un Eroe Evocato di una determinata rarità. Per ulteriori informazioni su questo argomento, visitate la pagina dell'argomento [Rarità](rarity.md).
