# Uso responsabile ed etico delle mappe

[**Lyzi Diamond**](https://twitter.com/lyzidiamond) - che attualmente è *docs lead* presso heroku, che in precedenza ha lavorato presso glitch, mapbox, maptimehq, codeforamerica e oregongeology - circa 10 giorni fa ha redatto un [*thread* twitter](https://twitter.com/lyzidiamond/status/1238556851643518981) molto bello sull'**uso** **responsabile** ed **etico** delle **mappe**, per evitare di **raccontare una storia sbagliata**.

Quando l'ha scritto era tra le pochissime che sottolineasse l'inadeguatezza di molte scelte di rappresentazione cartografica di tante mappe sul COVID19. Lei lo ha fatto a partire proprio da quella che ad oggi è stata più diffusa.
<br>Da quel giorno altre e altri si sono uniti.

Ci è sembrato e ci sembra ancora un contributo prezioso sul tema e abbiamo voluto crearne una traduzione in italiano. Un grazie a [Paola Masuzzo](https://twitter.com/pcmasuzzo) per il tempo che ha dedicato alla cosa.

## Il thread

Ciao a tutti, facciamo un altro Twitter-torial sulle mappe!
L'argomento di oggi è la **visualizzazione di dati aggregati**. Si tratta per lo più di una critica a [questa mappa](https://www.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6), che probabilmente avrete visto circolare un bel po'.<br>
È una mappa che mostra dati importanti! Ma ho qualche problema con le tecniche utilizzate.

[tweet originale](https://twitter.com/lyzidiamond/status/1238556851643518981)

---

Conosciamo tutti le mappe che visualizzano dati aggregati. La più nota tra tutte è probabilmente la [**mappa coropletica**](https://www.wikiwand.com/it/Mappa_coropletica): mostra aree geografiche riempite con un colore o un motivo, per rappresentare informazioni relative a quelle aree.<br>
Un esempio è questa elettorale della BBC:


![mappa coropletica](imgs/coropleta.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238556851643518981)

---

I colori sulla mappa rappresentano delle informazioni: ad esempio, quale partito ha vinto le elezioni in un distretto e con quale percentuale. Le mappe coropletiche hanno dei limiti (spesso legati a ipotesi fatte su aree geografiche estese), ma sono comunque utili per mostrare dati aggregati per aree.

[tweet originale](https://twitter.com/lyzidiamond/status/1238559830828253186)

---

Esistono altri due modi comuni di visualizzare dati aggregati: le “mappe a densità di punti”  e quelle con simboli di dimensioni variabili rispetto a una parametro. Le “mappe a densità di punti” usano un punto per rappresentare un determinato numero di elementi che si vogliono mappare, e raggruppano i punti in un’area geografica.
<br>Ecco un esempio di Bill Rankin (2009):


![mappa a densità di punti](imgs/dotDensity.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238560988619816963)

Ciascun punto rappresenta 25 persone nella città di Chicago. Ogni punto però non fornisce la locazione geografica precisa di quelle 25 persone, ma una posizione *random* dentro l’area geografica di interesse (assieme agli altri punti che appartengono alla stessa area geografica). Interessante, no? È di certo un bel modo per raccontare una storia.

[tweet originale](https://twitter.com/lyzidiamond/status/1238561449351557122)

---

Esistono anche le mappe a “simboli proporzionali”. In queste viene usato un simbolo (comunemente un cerchio) per rappresentare un’area geografica, e la dimensione e/o il colore del simbolo hanno una qualche relazione con una proprietà dei dati che si vogliono rappresentare. Un esempio: la mappa della diffusione del coronavirus sviluppata dall'istituto Johns Hopkins.

![mappa a simbolo graduato](imgs/graduatedSymbol.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238562354239078401)

Nel caso specifico di questa mappa, ciascun punto rappresenta uno stato/provincia o Paese (dipende dalla regione geografica, negli Stati Uniti d'America sono gli stati), e il raggio del cerchio di ogni punto cresce al crescere dei casi di coronavirus confermati in quell’area geografica. (Da notare che la scala non è lineare, ma logaritmica!)

![mappa a simbolo graduato - legenda](imgs/graduatedSymbolLegend.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238563186707697664)

---

Cosa ci vuole dire questa mappa? Lo scopo sembra voler essere quello di mostrare (e quindi informare l’utente su) il numero totale dei casi di COVID-19 nel mondo. La domanda è: ci riesce? La risposta? Sì e no. Ecco alcune mie critiche su questa mappa.

[tweet originale](https://twitter.com/lyzidiamond/status/1238563754922643458)

---

1 **Conoscere** il **numero** totale di casi in una **determinata** **area** geografica è **utile**. Conoscere il **numero** totale di casi entro una **specifica area politica**… forse un po’ **meno**. Se vivo al confine tra Washington e Oregon (supponiamo a Portland), quel confine di stato per me non ha molto significato…

[tweet originale](https://twitter.com/lyzidiamond/status/1238564009672085510)

---

In termini di contenimento e misure adottate da uno specifico stato, sembra essere utile sapere quanti casi sono presenti al suo interno. Da un punto di vista **epidemiologico**, però, ai virus **non** **importa** granché di **confini** di **stato**. Si parla infatti di un concetto chiamato il “**Problema  delle  unità areali modificabili**”.

[tweet originale](https://twitter.com/lyzidiamond/status/1238564199128879105)

---

Questo problema riguarda il modo in cui la modifica dei limiti delle aree di studio può cambiare completamente i risultati di un'analisi spaziale. Questo conduce ad un **errore** **ecologico**: l'idea che questi confini abbiano importanza nell’interpretazione dei dati (per saperne di più, guardate questo [Twitter-torial](https://twitter.com/lyzidiamond/status/1069342932249899008)).

[tweet originale](https://twitter.com/lyzidiamond/status/1238564846574145536)

---

La mia modesta opinione, quindi, è che mostrare il numero di casi per area geografica è utile, ma solo in termini di risposta "ufficiale" di quell’area geografica/amministrativa (risposta ai dati che si stanno interpretando).

[tweet originale](https://twitter.com/lyzidiamond/status/1238565387647754241)

---

2 Questa è una mappa “slippy”, il che significa che posso scorrerla, ingrandirla e rimpicciolirla. Una cosa utile! Posso quindi fare zoom sulla mia città per verificare se ci siano casi riportati. Vivo a New York, dove so che ci sono casi. Ma cosa succede quando aumento lo zoom?


![mappa - zoom in](imgs/mappaZoom.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238565819916922880)

---

Non trovo niente! E sapete perché? Perché il simbolo graduato che rappresenta il numero di casi nello stato (stato=area geografica) è situato nel suo **centroide** **geografico**, triangolato approssimativamente tra Binghamton ed Oneonta.

![mappa - centroide](imgs/centroide.jpg)

[tweet originale](https://twitter.com/lyzidiamond/status/1238566350383169541)

---

Il centroide di un’area è la posizione media di tutti i suoi punti -- non è proprio il “centro” dell’area, ma ci si avvicina. Se stessimo parlando di una mappa analogica (di carta), tutto ciò avrebbe molto più senso. È molto più semplice leggere la mappa quando facciamo zoom out! Ma..

[tweet originale](https://twitter.com/lyzidiamond/status/1238566716034232320)

---

… se io non sapessi come funzionano le mappe con simboli proporzionali, se non sapessi come vengono costruite, e quale messaggio cercano di trasmettere… ipotizzerei che NYC non abbia nessun caso di COVID-19 e che tutti i casi di New York sono concentrati intorno alla città di Downsville, New York. È lì che si trova il simbolo!

[tweet originale](https://twitter.com/lyzidiamond/status/1238567073732866048)

---

Inoltre, i simboli graduati scompaiono quando si fa uno *zoom* in avanti oltre il livello 7. Questo vuol dire che, anche se credessi che tutti i casi di New York sono localizzati in quell’area,  non saprei nemmeno di preciso dove localizzarla, perché i simboli scompaiono sinché non si fa *zoom* indietro.

[tweet originale](https://twitter.com/lyzidiamond/status/1238567378461622273)

---

Dunque, come possiamo rendere questa mappa più chiara? Quali accorgimenti può prendere un cartografo per raccontare questa storia in modo più chiaro?

[tweet originale](https://twitter.com/lyzidiamond/status/1238567667935690752)

---

Un’opzione è quella di impostare dei **limiti** allo ***zoom***. Semplicemente, non lasciare che l’utente possa fare *zoom* in avanti oltre un certo livello. Questa impostazione farebbe capire all’utente che non ci sono dati disponibili oltre una certa risoluzione/scala, e allo stesso tempo chiarisce che i simboli rappresentano un dato aggregato.

[tweet originale](https://twitter.com/lyzidiamond/status/1238567978691702784)

---

Onestamente, però, non riesco a capire del tutto che cosa sta cercando di mostrare o di raccontare questa mappa. Mostrare i casi confermati aggregati per stato o nazione non mi sembra una cosa molto utile. Piuttosto, che **andamento** hanno i casi **nel tempo**? Come potremmo visualizzare questo andamento? E le **statistiche** **normalizzate** per **popolazione**?

[tweet originale](https://twitter.com/lyzidiamond/status/1238568410239377409)

---

Sono consapevole che questi dati sono recenti e non sappiamo di preciso quanto siano affidabili, e so che è importante ottenere quante più informazioni possibile, che ci aiutino a capire che cosa sta succedendo. Il problema è che tutte queste mappe sono **rischiose** perché **raccontano** **una storia sbagliata**.

[tweet originale](https://twitter.com/lyzidiamond/status/1238568692050464768)

---

Un consiglio generale: quando si aggregano dei dati, bisogna per forza di cose **rimuovere** **dettagli** e sfumature.
È nostra responsabilità, come cartografi, assicurarci di farlo in **modo** **responsabile** ed **etico**, in particolare **condividendo** la **metodologia** che adoperiamo e spiegando i **risultati** che otteniamo.

[tweet originale](https://twitter.com/lyzidiamond/status/1238569235711959051)

---

Inoltre, **L’ALFABETIZZAZIONE SULLE MAPPE È IMPORTANTE E DOBBIAMO CONTINUARE A FARLA E TRASMETTERLA, ANCHE NELL’ERA DI GOOGLE MAPS**.
Le mappe sono strumenti storici di oppressione e spetta a noi **essere** **critici** sulla visualizzazione dei dati di tutti i tipi, piuttosto che accettarla come un **dogma**.

[tweet originale](https://twitter.com/lyzidiamond/status/1238569653770780673)

