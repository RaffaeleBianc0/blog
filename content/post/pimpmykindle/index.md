---
title: "Pimp my Kindle"
description: "Elaborazioni di un ebook reader manco fosse un Ciao"
date: "2026-09-15"
lastmod: '2026-09-15'
categories: 
  - "tecnologia"
# image: "images/cover.jpg"
draft: true
---

Nel 2026 scopro per caso che sul [mio vecchio Kindle regalatomi 10 anni prima]({{< ref "kindle.md" >}}) posso installare [KOReader](https://koreader.rocks), un software opensource per leggere ebook che offre una tonnellata di possibilità in più rispetto all'interfaccia nativa, tra cui mi interessavano soprattutto queste:
- lettura di formati ebook aggiuntivi, soprattutto EPUB (standard di mercato, che per anni non è stato supportato nativamente dai Kindle)
- supporto al reflow dei PDF, per riuscire a leggere i PDF re-impaginati anche su uno schermo così piccolo e lento
- download di feed RSS e conversione in "libri" da leggere
- controllo tipografico avanzato (font, margini, kerning, orientamento dello schermo, e varie altre opzioni che il software Amazon non prevede)
- ricerca del termine evidenziato su dizionari multilingua scaricabili in locale, traduttore, e Wikipedia
- supporto a plugin per l'estensione ulteriore delle funzionalità - questa cosa da sola vale tutto lo sforzo, vedi sotto

Figurati se non mi vien voglia di provare!  
Ecco quanto ho fatto.  



# Jailbreak + installazione
Primo prerequisito è aver fatto il _jailbreak_ del dispositivo. È davvero facile e guidato passo dopo passo su https://kindlemodding.org.  

Nello stesso sito, la procedura termina con le indicazioni per installare KOReader, tramite un paio di comandi elementari da digitare direttamente sul Kindle.  



# Plugin
Una volta installato KOReader, la prima cosa da fare secondo me è installare il plugin [Storefront](https://github.com/ultimatejimmy/storefront.koplugin), perché consente di valutare/installare/aggiornare/rimuovere tutti gli altri plugin direttamente dal Kindle, senza doverlo tenere collegato al PC.

Ho ovviamente sperimentato un bel po' di plugin, soprattutto per modificare l'interfaccia utente, ma anche per altre funzioni collaterali.  
Ti elenco i plugin che sto usando ancora oggi, dopo opportuna scrematura - necessaria anche per evitare di appesantire troppo l'hardware molto limitato del mio vetusto Kindle.

[Bookshelf](https://github.com/AndyHazz/bookshelf.koplugin) è la mia "home" preferita, anche dopo aver provato gli eccellenti [SimpleUI](https://github.com/doctorhetfield-cmd/simpleui.koplugin) e [ZenOS](https://github.com/xZenLabs/zen-os) per qualche giorno. Si può usare anche solo come sostituto della funzione "Libreria" di KOReader, e usare una customizzazione della home separata, ma Bookshelf fa già tutto quello che mi serve.

_TODO: screenshot_

[Bookends](https://github.com/AndyHazz/bookends.koplugin) consente di personalizzare l'intestazione e il pié di pagina visualizzati durante la lettura, inserendo informazioni come tempo/pagine/percentuale lettura trascorso/rimanente/totale rispetto al libro intero, al capitolo corrente, al giorno corrente, o alla sessione di lettura corrente, progressbar di tutte queste informazioni, titolo autore del libro e del capitolo corrente, eccetera eccetera.  
C'è una libreria di preset molto nutrita, altrimenti si può creare il proprio preset direttamente sul dispositivo.

_TODO: screenshot_




_TODO: verificare sul Kindle quali ho attivi_



# Backup metadati in Calibre
La gestione ideale della propria biblioteca ebook locale si può fare usando [Calibre](https://calibre-ebook.com) su PC, questo valeva anche per il Kindle pre-jailbreak.  
Per Calibre segnalo [KOReader Calibre plugin](https://github.com/kyxap/koreader-calibre-plugin) che consente di importare i metadati di tutti i libri del dispositivo in Calibre: l'avanzamento della lettura, gli highlights, le note, i segnalibri. Lo vedo anche come un bel backup di tutte le informazioni a corredo di quello che leggo, fatto in locale (quindi indipendente da qualsiasi destino imposto da Amazon o altre piattaforme cloud che fanno la stessa cosa e che a volte spariscono o iniziano a chiedere soldi) e ottenuto con un singolo click.



# Archiviazione highlights in Obsidian
Infine, uno dei motivi più interessanti per scegliere un ebook come supporto di lettura per la saggistica secondo me è **archiviare i propri _highlights_ permanentemente**, cioè tutte le parti che ho sottolineato in tutti i libri, in modo da poter "ripassare" le parti significative quando voglio (e anche visualizzarne una random sempre diversa in Bookshelf/SimpleUI/ZenOS, così ripasso sempre qualche concetto utile).  
Per questa archiviazione mi piace usare [Obsidian](https://obsidian.md) sul PC, e per Obsidian esiste il [KOReader Highlights Importer Plugin for Obsidian](https://github.com/t5k6/obsidian-koreader-highlights) che estrae tutti gli highlights dal dispositivo e crea/aggiorna tutte le note nel vault in pochi istanti, popolandole anche con i metadati che descrivono il libro da cui gli highlights sono stati estratti.



# Conclusioni
Con questa configurazione sono completamente sganciato da entità online (Amazon, Goodreads) che prima erano in possesso dei miei libri e dei miei metadati, e ho tutte le funzioni che potevo desiderare legate all'esperienza di lettura.  
Credo così di sfruttare al massimo questo vecchio Kindle fino a quando l'hardware reggerà - batteria e schermo in particolare.
Quando sarà il momento di abbandonarlo, avrò tutta la mia configurazione KOReader + plugins + tutta la mia libreria + tutti i metadati già backuppati su PC, e sarà questione di poco traslocare tutto nel prossimo dispositivo.
