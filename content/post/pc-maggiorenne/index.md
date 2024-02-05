---
title: "PC maggiorenne"
date: "2024-01-13"
categories: 
  - "tecnologia"
image: "images/x60.jpg"
image: images/x60.jpg
toc: true
---


Useresti oggi un computer di DICIOTTO anni fa? Io lo ho fatto per qualche giorno e adesso te lo racconto, perché ho sotto le dita una tastiera che... mo' ti dico, aspetta.

Dato che le ferie invernali di inizio 2024 sono state all'insegna di influenze e malesseri, ne ho approfittato per fare un esperimento nerd di quelli che facevo da giovane.  
Ho preso questo IBM ThinkPad X60, un PC ultraportatile di quelli piccolini che piacciono a me e tenuto abbastanza bene, solo che è del 2006, ha 2GB di RAM e la CPU a 32bit. Insomma un osso. Per fortuna almeno dentro c'è un SSD, per dargli quel minimo di brio in più.

Perché mai comprare un aggeggio del genere oggi?  
Perché anche i nerd hanno i loro sfizi da soddisfare!

Il mio primo sfizio era possedere un ThinkPad pre-2012, sia per provare a scrivere un po' con la celebre "classic keyboard" e capire perché è considerata da molti appassionati la migliore tastiera della storia dei notebook, sia perché il look professionale-retrò di questi modelli è fighissimo e fosse per me lo terrei esposto come arredamento in casa.  
Il feeling amarcord dei tasti burrosi che cedono generosamente sotto le dita con questo "clak clak clak" da laboratorio di informatica universitario appagano il mio animo nerd, e continuo a scrivere di gusto.  
E così il mio primo sfizio è stato soddisfatto, facile facile.

Il mio secondo sfizio era capire se un computer appena maggiorenne può ancora essere utile. Non credo di aver mai usato in vita mia un PC così vecchio!

Questo X60 è arrivato con Win10 installato e "funzionante": le virgolette sono d'obbligo perché era totalmente inchiodato, quasi inutilizzabile, con attese snervanti praticamente dopo ogni click del mouse.  
Per sicurezza ho re-installato Win10 da zero: stesso risultato. Per avere un riferimento che userò più sotto, aprire LibreOffice Writer richiedeva 20 secondi. Qual è l'ultimo programma che hai usato aspettando per VENTI SECONDI che si avviasse?

Ma questa lentezza non è stata una sorpresa, tant'è che prima di decidere di comprare il portatilino avevo già studiato i prossimi passaggi, esplorando il mondo delle distribuzioni Linux a 32 bit ed eseguibili "live" da chiavetta usb, cioè senza installarle nell'SSD, così da testarle rapidamente.  
Ne sono uscito con una decina di nomi, le ho scaricate tutte e le ho provate.  
Alcune non vedevano la scheda wifi, alcune non facevano nemmeno il boot... non ho né le competenze né la voglia di risolvere questi problemi, per cui le ho cancellate man mano e ho confrontato solo quelle utilizzabili subito senza sbattimenti.

Alla fine ha vinto antiX Linux (https://antixlinux.com), per questi motivi:  
\- appena avviato occupa solo 115 MB di RAM (Win10 ne occupava 900) lasciando ampio respiro alle applicazioni che voglio usare  
\- è super-reattivo e pare quasi di usare un PC recente, al netto dell'estetica essenziale  
\- è organizzato in modo abbastanza logico, tanto che anche senza essere pratico di Linux riesco a trovare facilmente quello che mi serve  
\- arriva con una ricca scelta di software leggero pre-installato per tutti gli utilizzi più normali di un PC (e comunque installare altri programmi col suo gestore pacchetti è senza dubbio più facile che trovare e installare un programma in Windows)  
\- include già LibreOffice e Firefox in versioni 2023, che non sono proprio leggeri ma che avrei installato in ogni caso per stare tranquillo con la compatibilità con i file Word/Excel/eccetera e il rendering dei siti web - insomma il classico modello di utilizzo "office+internet", probabilmente quello principale di qualunque PC, e soprattutto di uno vecchio e piccolo come questo, con il quale di sicuro non ci si mette a fare montaggio video.

Riesumando qualche nozione base appresa molti anni fa su Linux, provo qualche comando da terminale, installo qualche programma aggiuntivo, tutto funziona senza problemi. Una goduria.  
Dopo queste prove positive nell'ambiente antiX live eseguito da chiavetta, decido che lo voglio adottare come sistema operativo definitivo su questo PC, e così clicco l'iconcina dell'installer sul desktop: una procedura facilissima che conserva tutte le modifiche fatte live (la password del wifi, il tema grafico, le applicazioni che ho aggiunto...) e che consente di compilare le informazioni necessarie all'installazione (nome utente, nome PC, fuso orario...) MENTRE questa sta andando in background, invece che alla fine: tempi morti azzerati, e in meno di 5 minuti antiX è installato nell'ssd e pronto per l'uso (Win10 ci ha messo mezz'ora abbondante, più una decina di minuti aggiuntivi a fare domande su quanto vuoi essere profilato mentre lo usi, e a mostrare "Ci siamo quasi" e altre frasi del cacchio a schermo intero mentre aspetti che finisca non si sa bene cosa, più un altro paio d'ore per completare gli aggiornamenti dopo l'installazione).

E arrivo così al punto del mio esperimento: ho usato questo ThinkPad per qualche ora "da utente", cioè non per cincionare sul sistema ma per scrivere, navigare, un po' di Facebook YouTube Reddit Wikipedia, salvare file sulla chiavetta e riaprirli, eccetera eccetera.  
Le applicazioni locali funzionano bene, quelle più moderne (versioni 2023 di LibreOffice, Firefox, Chromium) sono ovviamente lente ad avviarsi e meno reattive che su un PC moderno. LibreOffice Writer per esempio parte in 10 secondi - che è comunque la METÀ di quanto ci metteva in Win10 a parità di versione e di PC.  
I siti web più complessi, come Facebook e YouTube, sono una vera sfida per questa macchinetta, e spingono spesso al 100% la CPU anche solo per caricare le immagini e fare lo scrolling della pagina, rendendo tutto un po' scattoso: probabilmente le tecnologie usate per realizzare le pagine web dinamiche più complesse richiedono molta elaborazione lato client. Per confronto, Wikipedia, che è un sito con pagine molto più semplici, si naviga senza rallentamenti.  
I video YouTube si vedono senza perdita di fotogrammi in Chromium, ovviamente ridotti a 720p data la risoluzione limitata del display, ma con la CPU che oscilla tra il 60% e il 100% di carico, quindi siamo proprio al limite (mentre in Win10 è stato impossibile vederne uno senza un buon 20% di fotogrammi persi).

Complessivamente riassumerei dicendo che si può usare un PC di 18 anni fa per fare normali attività in ambito office+web, a patto di usare una distribuzione Linux leggera. Non è ovviamente tutto fluido e reattivo come su un PC moderno, ma è utilizzabile. Windows 10 invece è troppo pesante per un hardware così limitato.  
Un PC un po' più recente risolve il grosso dei problemi di lentezza, spesso anche senza abbandonare Windows, come ho già sperimentato negli ultimi mesi con una decina di computer diversi degli anni 2013-2018 che mi sono passati per le mani.

Questa esperienza mi riporta alla mente riflessioni già fatte molte volte sull'obsolescenza programmata, sulla foga dell'aggiornamento a tutti i costi, sulla diffusione di Windows che, in tanti dettagli che non ho scritto per non appesantire troppo il testo, mi è sembrato un sistema operativo inferiore a Linux. Chissà quanti PC sono stati rottamati dopo pochi anni perché "è diventato lento e mi sono preso il computer nuovo".  
PC vecchi, anche così vecchi come questo ThinkPad diciottenne, una volta sostituito Windows con Linux possono essere rimessi in gioco e usati per web, email, chat, consumo di media, scrittura, didattica, e chissà quante altre cose. Magari hanno la batteria esausta, magari non hanno le porte più recenti per collegarci i dispositivi moderni, magari sono un po' grossi/pesanti, eccetera eccetera... ma se proprio non me ne faccio nulla lo può usare il nonno, o la mamma, o una scuola, o un'associazione. Anzi se avete qualche input su questa cosa delle associazioni fatemi sapere, è da un po' che mi stuzzica l'idea di poter dare una mano. L'importante è non buttarli via.

Paura di Linux perché "è complicato, è roba da smanettoni"?  
E se fosse solo un vecchio pregiudizio?  
Alla fine il modello "desktop finestre icone menu tastodestro copia-e-incolla eccetera" degli ambienti desktop Linux più diffusi è proprio quello al quale siamo abituati da decenni con Windows, e in ogni caso quello che facciamo con un PC si è spostato parecchio sul web, quindi dopo che hai lanciato il browser le differenze con Windows non le vedi neanche.

Bello bello davvero, ho imparato qualcosa di interessante e mi sono divertito assai!
