---
layout: default
titolo: Primo Documentazione del prototipo
category: documentazione
---

<div id="edit"> <a href="http://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md">Modifica questo documento</a></div>

<div id="notes">
	Questa è la prima bozza della documentazione di Primo, pubblicata il 28 febbraio 2014. <br>
	Il codice Arduino non è incluso in questa versione perché stiamo ancora perfezionandolo, ma sarà presto reso pubblico. Visita spesso questa pagina perché sarà aggiornata giornalmente con dei nuovi contenuti.
	<br><br>
	<a href="http://github.com/primo-io/prototype-documentation">Vedi su GitHub</a>
</div>

##0. Cosa è questo documento?

![primo play set](images/photo/maker-guide.jpg)
Questo document raccoglie e organizza tutte le informazioni necessarie per costruire un prototipo di Primo.
Se vuoi saperne di più su Primo visita il sito ufficiale: [primo.io](http://primo.io) 

##IMPORTANTE
La documentazione e le istruzioni incluse in questo documento permettono di realizzare un prototipo di Primo così come appare in questo video, in una versione differente dal prodotto finale. Parallelamente, continueremo a pubblicare la documentazione necessaria riguardo agli aggiornamenti e alle nuove versioni del Primo Play Set, e a includere i file del prodotto finale, solo dopo averli testati.


##MOLTO IMPORTANTE
La licenza che abbiamo scelto per pubblicare Primo Play Set ti permette di costruire un tuo prototipo. **Tu non hai diritto a venderlo come Primo**, in nessuna circostanza. Inoltre, se crei un derivato del nostro prodotto, devi sempre indicare Primo come progetto originale (come facciamo anche noi con tutte le nostre risorse), e usare la nostra stessa licenza: [CC by-nc-sa 4.0 International](http://creativecommons.org/licenses/by-nc-sa/4.0/). <br>
Questa procedura non deve essere applicata solo per proteggere la nostra proprietà intellettuale, ma per tenere traccia del flusso delle idee. Visto che stiamo investendo molto tempo e risorse per fare in modo che questa documentazione sia gratuita e accessibile, ti incoraggiamo a "rendere" e pubblicare il tuo derivato, i risultati, i suggerimenti, gli insulti e gli elogi. Siamo molto felici di ricevere e rispondere 8 and blog cool stuff.

###Come tradurre questo documento

If you want to translate this page in your language, you have multiple options, depending on your .

1. (super easy, no automation) The easiest one, is to copy and paste this page in your text editor, translate it then mail it to us at [play@primo.io](mailto:play@primo.io)

2. (medium, light automation) Another very easy option is to create an account on [GitHub](http://github.com), then open the [repository of this page](https://github.com/primo-io/prototype-documentation/blob/gh-pages/index.md) and click on 'EDIT', in the top menu bar:
![photo](images/screenshots/edit-1.jpg)
Then your page turns into a text editor, where you are able to modify the page source. The page is written in [markdown](http://daringfireball.net/projects/markdown/syntax), very easy to understand. 
![photo](images/screenshots/edit-2.jpg)
You don't have to modify this code, but just copy and paste the whole text in your local text editor, then translate the textual parts in your language, without modifying the parenthesis and HTML parts. Save the text then mail it to us at [play@primo.io](mailto:play@primo.io)

3. (advanced, full automation) This is slightly advanced, but nothing too hard, if you are not familiar with GitHub you have the chance to learn something new :) 
Ig you are already familiar with git, in a few words you have to copy the 


##1. Che cosa è Primo

![primo play set](images/photo/primo.jpg)

Primo è un'interfaccia tangibile progettata per spiegare la logica della programmazione a bambini dai 3 ai 7 anni, ovvero nell'età pre alfabetismo. Obiettivo del gioco è di fare in modo che una piccola macchina robot chiamata Cubetto torni a casa. Per completare il gioco, i bambini devono programmare il piccolo robot attraverso una serie di istruzioni: avanti, sinistra, destra e funzione. Le prime tre istruzioni sono abbastanza intuitive, mentre l'ultima - la funzione - va a richiamare una "sub-routine", ovvero quello che in programmazione è un'insieme di istruzioni compresse in un unico comando. 

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/82620072" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe> 
</div>

##2. La ricerca alla base del progetto Primo

L'insegmanento della programmazione ai bambini è un argomento ampiamente dibattuto. Esistono alcune soluzioni che cercano di supportare questo tipo di attività, ma solo per bambini di età superiore agli otto anni. Al di sotto di questa età, esistono invece poche soluzioni e quasi tutte sono basate sull'uso di uno schermo e sulla necessità di essere alfabetizzati. E' possibile trovare un numero di Apps per tablet e applicazioni per il computer che sono combinate con robot fisici, ma nessuna di queste offre delle funzionalità che siano completamente libere dall'uso di "pixel" come Primo.

Il legno è stato scelto come materiale principale del prodotto in primo luogo perché è naturale; il contatto con il legno offre una sensazione calda e il suo suono è morbido. Il legno è stato scelto anche per un motivo culturale. Abbiamo condotto delle ricerche basate sull'osservazione degli asili in Svizzera (dove il prodotto è stato inizialmente) e abbiamo scoperto che i giochi piu' usati e amati dai bambini sono quelli costuiti con il legno. I giocattoli di legno durano molto e conservano su di essi i graffi e i segni che mostrano l'uso degli altri bambini nel tempo. E' un materiale che conserva ricordi. Il legno è stato scelto anche perché contrasta la freddezza della tecnologia. All'interno di Primo c'è un circuito e dell'hardware, ma è stato nascosto per ricreare un'esperienza "magica" che nasconde la complessità del gioco.

<img class="float" src="images/photo/logo-turtle.jpg">

Il concetto di Primo si ispira fortemente al lavoro di Seymour Papert, un matematico che ha cofondato il MIT Artificial Intelligence Laboratory insieme a Marvin Minsky, durante gli anni sessanta (se siete interessati a saperné di piu' vi incoraggiamo a leggere [Mindstorms](http://www.amazon.co.uk/Mindstorms-Children-Computers-Powerful-Ideas/dp/0465046746/ref=sr_1_1?ie=UTF8&qid=1393675158&sr=8-1&keywords=mindstorms+papert), il suo libro piu' famoso). Seymour ha diretto il gruppo che inventò[LOGO](http://en.wikipedia.org/wiki/Logo_(programming_language)), probabilmente la risorsa più usata e valida ancora oggi per insegnare la programmazione ai bambini. L'obiettivo di Seymour Papert non era di insegnare solo la parte relativa al codice, ma anche di insegnare ai bambini a scoprire da soli come risolvere problemi. 
Primo puòn essere considerato come un progetto di semplificazione di LOGO e della sua tartaruga fisica. 
In Primo le istruzioni sono ridotte alla forma piu' pura per evitare ogni tipo di linguaggio basato su testo e numeri.

Il primo prototipo è stato realizzato alla SUPSI - Scuola universitaria professionale della Svizzera italiana - da Matteo Loglio (co-fondatore e interaction designer di Primo.io ), durante il [MAInD - Master of Advanced Studies in Interaction Design](http://www.maind.supsi.ch/). Matteo ha una formazione in product design, e dopo aver imparato le basi di Arduino basics e un pò di programmazione per creare prototitpo, ha iniziato a cercare delle soluzioni tecniche che permettessero a delle persone non esperte di sviluppare applicazioni come, per esempio, Primo. In questa ricerca i problemi principali erano due: realizzare un robot dal principio e un'interfaccia fisica che potesse riconoscere facilmente varie istruzioni.

Il primo problema è stato risolto attraverso l'uso della scheda [Oh_Oh board](http://david.cuartielles.com/w/Maquila2/Ohoh) realizzata da David Cuartielles, uno dei fondatori di Arduino che aveva partecipato ad un seminario alla SUPSI. Il robot Oh_Oh è un progetto open source: potete trovare i file sorgente cliccando il link sopra. Il robot è essenzialmente un Arduino a forma di macchinina con un Xbee per gestire la comunicazione radio.

Il secondo problema è stato progettare un sistema stabile per riconoscere i blocchi (istruzioni). La soluzione usata per Primo è ispirata a un progetto sviluppato presso il [CIID](http://ciid.dk/) chiamato ["Barcode Piano"](http://ciid.dk/education/portfolio/idp11/courses/physical-computing/projects/barcode-piano/). 

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/19704918" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div> 

L'idea è di usare vari blocchi che possono essere riconosciuti dalla board attraverso delle resistenze, ovvero un voltage divider con le pin analogiche di Arduino che leggono i valori delle resistenze. Un metodo molto semplice, ma molto efficace per realizzare un prototipo.

Dal punto di vista del design, alcune funzionalità dovevano essere testate; il design attuale è il risultato di diverse iterazioni. 

Il percorso a 'serpente' o 'zig-zag' della sequenza di istrizioni è stato scelto per evitare che l'utente abbia bisogno di concetti di alfabetismo.  

![left to right](images/illustrations/left-to-right.jpg)

La forma a 'D' dei blocchi "connettori" è stata progettata in modo che i blocchi potessero essere inseriti solo in un verso, al fine di renderli consistenti con il design del percorso e la direzione della macchina. Design molteplici possono essere utilizzati per questa parte del gioco. La forma a D è stata scelta soprattutto perché è un 'cerchio oeriented' e perché richiama il design di altre board che usano dei blocchi.

![instruction blocks](images/photo/instruction-blocks.jpg)

The design della forma dei blocchi 'istruzione' deve ancora essere testata. Il design attuale funziona abbastanza bene, i bambini facilmente riescono a comprendere la loro funzione, ma hanno solo dei problemi durante il primo uso a capire la differenza tra i blocchi a sinista e quelli a destra. Questo succede anche perché il concetto di 'destra' e 'sinistra' è qualcosa di nuovo a quella età. Stiamo attualmente testando dei nuovi design per i blocchi al fine di migliorare questo aspetto.

<div class="videoWrapper">
	<iframe src="//player.vimeo.com/video/50570097" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

Al principio, il robot era una macchina la cui realizzazione era molto complicata e dispendiosa in termini di tempo: era composta da strati di legno tagliati al laser e incollati uno per uno e successivamente cartavetrati per più di un'ora. La macchina aveva anche un altro problema: sembrava solo per maschietti. Abbiamo voluto evitare di creare discussioni riguardo alla produzione di giocattoli per maschi e essere criticati per questo. Abbiamo deciso, quindi, di restare neutri e creare un prodotto indirizzato sia ai bambini, così abbiamo optato per una geometria semplice, ovvero una scatola.

Abbiamo dato un nome alla piccola scatola e una personalità tramite ad un volto sorridente, rendendolo molto attrattivo per i bambini. Il robot è stato chiamato Cubetto. L'idea alla base di Cubetto è di offrire un modulo di base che può essere modificato e personalizzato facilmente in futuro.

![cubetto](images/photo/cubetto.jpg)

##3. Per iniziare

###3.1 Le componenti di base

Primo è composto da tre parti: una interfaccia fisica, Cubetto e il set di blocchi 'istruzione'. I bambini interagiscono con l'interfaccia fisica inserendo i blocchi nei fori, creando una sequenza (il programma A) che Cubetto esegue. 

Ci sono quattro tipi di blocchi e questo vuol dire che devono essere usate le resistenze di quattro valori differenti, possibilmente distanti l'uno dall'altra. 

I blocchi devono essere inseriti nei fori dell'interfaccia fisica dove è rilevato il valore delle resistenze. Dopo il riconoscimento, i valori sono elaborati in una sequenza di caratteri che è inviata a Cubetto attraverso il modulo XBee. Cubetto poi esegue le istruzioni, una dopo l'altra. 

Il cervallo del prototipo è basato su due schede Arduino, una UNO (o una Leonardo o una Duemilanove funziono ugualmente) per Cubetto e una Mega per l'interfaccia fisica per la quale sono necessari 16 pin per gli input analogici.

###3.2 L'elettronica

###Strumenti necessari

* Saldatore
* Stagno
* Cavi
* Pistola con colla a caldo
* Colla per il legno
* Nastro di rame di larghezza 5 mm

###Materiali (prezzi in euro)

Cubetto ~ 88 €

* Arduino UNO (o Leonardo) - 20 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=195#.UxC5nfTV_bA)
* Arduino Proto Wireless Shield - 14.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* SN754410 Motor Driver - 3.90 € : [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_33&products_id=153#.UxC5-_TV_bB)
* XBee (serie 1 or 2, non c'è differenza) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* SolarBotics ruote x 2 : 4.74 € - [Solarbotics Store](https://solarbotics.com/product/gmpw/)
* SolarBotics Gear Motors GM3 x 2 : 8.36 € - [Solarbotics Store](https://solarbotics.com/product/gm3/)
* 2 Ball Casters : 5.79 € - [Solarbotics Store](https://solarbotics.com/product/23160/)
* CNY70 x 2 : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Vishay/CNY70/?qs=%2fha2pyFaduj8YpDhNNtXszq4w32cl%2fAjUjdOwQUvJUM%3d)
* (optional) Battery Holder: 4 € - [Solarbotics Store](https://solarbotics.com/product/bholdaa_4_cell/)
* (optional) 4 x Batterie ricaricabili

Interfaccia fisica ~ 88 € (solo una coincidenza)

* Arduino Mega 2560 : 39.00 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=11&products_id=196#.UxC_gPTV_bA)
* Arduino Proto Wireless Shield : 14.90 - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_5&products_id=145#.UxC53vTV_bA)
* XBee (series 1 or 2, doesn't make any difference) : 23.90 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=37_38&products_id=292#.UxC6cvTV_bA)
* 16 5mm Red LED : 1 € - [Mouser](http://uk.mouser.com/ProductDetail/Lite-On/LTL-4223/?Lite-On/LTL-4223/&qs=sGAEpiMZZMusoohG2hS%252b15J8d1kHl%252bvkJpzS4atZNEA=)
* 16 220 Ω Resistors : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 16 10K Ω Resistors : 0.16 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 1 Push Button : 1 € 
* 50 Male Headers : 1 € 
* 16 Double male headers : 0.50 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=294#.UxC_3fTV_bA)
* 50 female headers : 1 € - [Arduino Store](http://store.arduino.cc/index.php?main_page=product_info&cPath=6_32&products_id=188#.UxDAAfTV_bA)
* 16 Magneti ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

Blocchi ~ 4 €

* 4 x 4.7K Ω Resistenza : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-47K-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2fbdyz6pU6a%252bvHlD5kaZWgo%3d)
* 4 x 100K Ω Resistenza : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-100K-RC/?qs=sGAEpiMZZMu61qfTUdNhG81NIhcRRUJQxII5Nsctha8%3d)
* 4 x 220 Ω Resistenza : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-220-RC/?qs=sGAEpiMZZMu61qfTUdNhG%2f1uGo5nxyCVqn6ChOCvUEE%3d)
* 4 x 10K Ω Resistenza : 0.04 € - [Mouser](http://uk.mouser.com/ProductDetail/Xicon/291-10K-RC/?qs=sGAEpiMZZMu61qfTUdNhG6xwTrVwTvbz8PPav3aExs8%3d)
* 16 Magneti ø 4 h 3 : 3.5 € - [Supermagnete](http://www.supermagnete.ch/eng/S-04-03-N)

###3.3 Alimentazione

Cubetto e (opzionalmente) l'interfaccia fisica, sono alimentati tramite batteria. Per il prototipo, è possibile usare una batteria LiPo or una batteria normale AA, a scelta. Noi abbiamo usato entrambe, le batterie LiPo sono buone, ma non richiedono l'utilizzo di componenti aggiuntivi. Se state iniziando da zero, suggeriamo di usare le batterie AA. Considerate solo che si consumano molto velocemente, quindi, la soluzione migliore è usare batterie ricaricabili come le NiMh.

###3.4 Design del prototipo

L'intero prodotto è fatto con legno tagliato con una macchina laser, 4mm di spessore, con un solo strato di spesso 1mm.  Potete tagliare queste parti usando servizi come Ponoko, o presso il fablab più vicino a casa vostra. Il primo prototipo è stato tagliato al [FabLab Lugano](http://fablab.supsi.ch/), mentre lo sviluppo avanzato del prodotto al [FabLab Torino](http://fablabtorino.org/), dove vive e lavora ancora una parte del team di sviluppo. 

Costuire Cubetto and l'interfaccia fisica è abbastanza laborioso, ma la procedura è abbastanza semplice: le scocche sono semplicemente delle scatole! La parte più complessa è l'assemblaggio dei blocchi che sono costituiti da un doppio strato di legno con spessore 4mm e magneti e resistenze saldate al suo interno.

##4. Realizzare il prototipo

###[Scarica i file sorgente](files/primo-prototype-laser.zip)

###4.1 L'interfaccia fisica

Per are l'interfaccia fisica, dovete tagliare al laser due file, interface-board-4mm.dxf e interface-board-1mm.dxf: il primo file serve per lavorare il compensato di spessore 4mm e il secondo per il compensato di 1mm. Come potete vedere dai file, le parti sono numerate per facilitarvi nel processo di assemblaggio. I numeri sono indicati in un livello diverso per permettervi di rimuoverli facilmente prima di tagliare il file con la macchina laser. Vi suggeriamo di verficare e modificare la grandezza dei fori che deve essere adeguata alla grandezza del bottone che intendete usare o che avete. 

Prima di tutto, dovete incollare le parti numero 3 e numero 4 e usare i fori negli angoli per allinearle con le viti mentre versate la colla. Poi, dovete lasciarle a riposo per una notte. 

Dopo, prendete il nastro di rame, tagliate 32 pezzi di larghezza 70 mm ciascuno e poneteli all'interno thei fori rettangolari sulla zona che avete appena incollato. Verficate che stiano almeno a 30mm da ogni lato. Once you finished, you can now glue all the remaining top layers of the interface board, this is the correct order:

Then take the copper tape, cut 32 pieces of 70mm each and put them inside the rectangular holes in the part that you just glued, they should be at least 30mm wide on each side. 

![copper connectors](images/illustrations/board-1.jpg)
![copper connectors](images/illustrations/board-2.jpg)

Once you finished, you can now glue the previously glued parts, 1+2 with 3+4.

![copper connectors](images/illustrations/board-esploso.jpg)

Once the glue has dried, put the magnets in the little holes. Turn your top layer upside-down and fill the little holes with the magnets, make sure they are all in the same direction, doesn't matter if north or south. Seal the hole with a drop of hot glue.

Now the electronics. Start by making rails for the 5V and the GND, all along the hole lines like in the picture. The first ever prototype never had copper strips, it had wires (which you can also use), but in this prototype we used copper tape also for the rails. A real 100% time saver. It also makes things easier for creating connections.

![rails](images/illustrations/board-3.jpg)

The next step is to wire one of the two connectors of every hole, to the ground rail. If you used copper tape, you can just use a tiny extra bit of it, just enough to touch both ends.

![rails](images/illustrations/board-5.jpg)

Now we have to connect the other side of each connector to the 5V rail, but this time, with a 10KΩ resistor in-between. A cool thing of copper tape is that solder melts very well on top of it. This is the technique used:

![10k](images/photo/diy-docs-1.jpg)

At the end of this process, you should have something like this:

![10k scheme](images/illustrations/board-6.jpg)

Now it's time to put the LEDs; stick one red LED in each one of the 16 holes, then use a drop of hot glue to seal them to the wood. Once the glue is cold, we have to connect them. Just mind that LEDs have a polarity: the long leg is the anode and the short one the cathode. Connect each cathode to the ground rail, using a 220Ω Resistor.

![10k](images/photo/diy-docs-6.jpg)

Connect each cathode to the ground rail, using a 220Ω Resistor.

![10k scheme](images/illustrations/board-7.jpg)

The long leg of the LED, must be connected to a digital I/O pin on the Arduino Mega, these pins are numbered from 22 to 53. The LEDs must be connected in order, so that it will be much easier to access them later on in the code, in my prototype for example I started from pin number 30 up to 45 (there are 16 LEDs). 
The starting point is not important, as long as they are in the correct sequential order. This means for example that if we start from pin 30, the first LED must be attached to pin 30, the second to pin 31, the third to pin 32 and so on until LED 16 to pin 45. 

The cables are soldered to a rack of double male headers, as the digital pins on the Arduino Mega are laid out in a double line. In this way it's easy to plug and remove the Arduino from the board.

![rack](images/photo/diy-docs-4.jpg)

Once all the LEDs are soldered, we have to solder our hand made connectors. These must be wired to the Arduino Mega analog pins, to read the different resistor values. Just like the LEDs, these must be connected in order, starting from A0 for hole 1 to A15 for hole 16. The wire has to start from the same point where we soldered previously the 10K resistor. See the illustration:

![analog input board connections](images/illustrations/board-8.jpg)

<div class="cf">
<img class="float cf" src="images/illustrations/button.jpg">

<p>
Here I used some single male headers, as the analog pins are all on a single line.
	
</p>

<p>
The last thing to connect is the button: take it and solder two cables to two opposite headers, then slip them trough the button hole, from the top, and push it all the way down, until it stops. Now flip the board, you should have the two wires coming out of the hole. Connect them as in the illustration: one straight to 5V, the other one to GND using a 10k Resistor. Then connect it to an Arduino digital pin from the button-end of the resistor, in this example we used pin number 50.
</p>
</div>


![photo](images/photo/diy-docs-5.jpg)

Almost done with the board, now you just have to plug the Wireless Shield on top of the Arduino Mega and stick the headers in place in the board. To recap, 30 to 45 for the LEDs, A0 to A15 for the connectors and 50 for the button. Use the A0 to A5 pins on the Wireless Shield for the first 5 connectors. Don't forget to connect the ground rail to the GND pin and the 5V to the 5V pin.

![rack](images/photo/diy-docs-3.jpg)

Now a little bit of fine-tuning: after that part 12 of the board has been painted, you can glue it with part 13 on top of the board.

Same for the red button: after part 14 has been painted, put something soft like cardboard on top of part 2, around the push button, then some hot glue on top of the push button and before the glue dries off, place the red button. See the illustration:

![photo](images/illustrations/button-mechanics.jpg)

###INSTRUCTION BLOCKS

This is one instruction block, exploded:

<img class="float cf" src="images/illustrations/instruction-esploso.jpg">

To make the Instruction Blocks, the first thing you have to do is laser cut the files, there's one for 4mm thick wood and one for 1mm wood. They are four layers, numbered from 1 to 4 and the drawings provided can be used to make 16 blocks, four of each kind.

Each block has a different resistor. These are the resistors used in the prototype:

FORWARD: 4.7K Ω<br>
LEFT: 100K Ω<br>
RIGHT: 220 Ω<br>
FUNCTION: 10K Ω

To make blocks, first you have to glue part 4 with part 3. 

After the glue has dried, you can start painting. See the illustration below to see what part should be colored:

![image](images/illustrations/colors.jpg)

Now you have to cut two pieces of copper tape, 40mm long. Slip them in the holes of the two blocks that you just glued, making a ring around it using the upper and lower fissure, the ring must be quite tight.

![photo](images/illustrations/instruction-block-guide.jpg)

After that, you have to put the magnet in the hole. While doing this, BE SURE THAT IT IS CORRECTELY ORIENTED, so that the block 'sticks' into the hole. If you put it the other way, it's going to be repelled by the other magnet, a funny outcome but not what we want to achieve.

Fix the magnet with a drop of hot glue and before the glue gets cold, put the right resistor on top, with the 'legs' laying on the copper tape. After that, the resistor must be soldered on the two pieces. After soldering, cut the extra leg length and glue part 2 on top of the resistor.

Finish your block by gluing the last layer, part number 1, on the top, then repeat the entire process for every single block :)

###CUBETTO

Electronics:

The prototype for Cubetto can be built using an Arduino Uno or Leonardo, with a Proto Wireless Shield on top. The reason for the Proto Shield is because it has a small prototyping area, that is wide enough to put the motor driver, the connectors for the optical encoders, motors and power. 

Cubetto has to spin 90 degrees left and right. A very inaccurate way is to use timing event, like "spin right for one second" and you can expect more or less the same result. "More or less" because it depends a lot from different factors, such as the floor, the battery power and so on. The way I solved this problem, is by detecting the amount of rotation from the wheel using two CNY70 optical encoders in combination with a sticker. The round sticker goes in the inner wheel and it's something like this:

![photo](images/photo/diy-docs-14.jpg)

The sticker is split into black and white slices, this is because the CNY70 is able to detect the variation between a white slice and a black one. Basically inside it has an infrared LED that is always on and a phototransistor that is reading the amount of infrared light. When a black material is facing the component, almost no light is relfected, as the black color tends to absorb it. On the contrary, if the material is white, it reflects all the light, so the value read from the sensor it's very high. The difference between readings is used to count the rotation steps.

![photo](images/illustrations/cny70-physycs.jpg)

The prototyping area of the Wireless Proto Shield is where the motor driver and other connectors for the other parts are soldered. For these, simply use male headers as connector and female headers on the other part.


![photo](images/illustrations/wireless-shield-connections.jpg)

For these I used simple male headers as connector and female headers on the other part.

![photo](images/photo/diy-docs-12.jpg)

![photo](images/illustrations/wireless-shield-connections-1.jpg)

The SN754410 motor driver has 16 pins that must be connected following this scheme:

![photo](images/illustrations/motor-driver.jpg)

Design:

Start by lasering cubetto.dxf; All Cubetto parts are cut from 4mm plywood, follow these visual instructions to build the base:

![photo](images/illustrations/cubetto-guide.jpg)

Don't mount the motors for now, first you have to mount the ball casters.

![photo](images/illustrations/ball-caster.jpg)

![photo](images/photo/diy-docs-9.jpg)

Now the CNY70. Solder the two opposite headers, that must be connected to 5V, together with a wire; then solder three wires to the remaining headers of the CNY70. At the end of these wires solder a row of three female headers. They will later be connected on to the headers of the proto shield.

The two cny70 must be placed on the edge of the bottom layer, with the LED and the photoransistot horizontally aligned. To fix them you can use some hot glue (or other types of glue). 

See the picture to understand the location.

![photo](images/photo/diy-docs-11.jpg)

Just like for the CNY70, solder two wires to the little flaps that come out of each motor. You can twist the two wires to make them more resistent, then at the end, solder a row of two female header, just like in the illustration.

Now print the inner drawing with the black and white slices, glue them on a piece of cardboard (or laser cut wood, that's up to you), cut the perimeter and make a hole in the middle, as they will be inserted between the motor and the wheel. The white and black slices must point towards the inner side of Cubetto and the distance between the print and the CNY70 must be between 1 and 3 millimeters for the CNY70 to work properly.

![photo](images/photo/diy-docs-10.jpg)

Now you can put the wheels on the motors, if you used the Solarbotics wheels, you can fasten them with the screw provided, don't make it too tight. 

Glue three out of the four 'walls' of Cubetto, parts 5, 7 and 8. We are going to leave the back removable, just in case we want to modify something. 

Take the battery holder and solder the black and red cable to other 2 female connectors. The headers on the shield will go to VIN and ground. A switch that breaks the red wire is heavily suggested.

![photo](images/photo/diy-docs-13.jpg)

Now you can place the Arduino + Proto shield on top of the motors, plug all the headers on the shield and you have finished making Cubetto.
