---
title: "Hugo"
date: "2024-02-09"
categories: 
  - "tecnologia"
image: "images/hugo-logo.png"
---

Benvenuto nel mio blog.

Ogni tanto lo rivoluziono perché lo uso anche come palestra per smanettare con qualche strumento nuovo.

Ecco la storia di questo sito, da quando è nato ad oggi.

## 1996: HTML statico

Era circa il 1996, avevo iniziato l'università e, grazie al laboratorio di informatica, muovevo i miei primissimi passi su Internet. Ricordo ancora la sensazione provata scambiando i primi messaggi online con ignoti, dall'altra parte del mondo, in inglese, parlando di batteria, scrivendo sui newsgroup Usenet con pine, un software a caratteri che si usava sulle SPARCstation UNIX che c'erano al [DEI](https://www.dei.unipd.it)!

Appena ho capito che potevo avere un mio sito personale online ho imparato a farmelo, anche se a livello molto rudimentale. Erano i tempi dell'HTML scritto a mano con un editor di testo, poi sostituito dalle prime versioni di Dreamweaver per aiutare con il layout. Al tempo non li chiamavamo ancora "blog", forse non esistevano nemmeno in Italia, li chiamavamo proprio "siti web".

## 2000: forum su e107

La prima versione "dinamica" del mio sito vide la luce nel periodo d'oro dei forum online, nei primi anni 2000: imparai ad installarmi Apache, MySQL e PHP, e testai qualche CMS opensource, cercando le informazioni su [www.opensourceCMS.com](https://www.opensourcecms.com).

Ne scelsi uno che si chiamava e107, ma non ricordo bene il motivo di questa scelta. Ci smanettai in modo da ottenere il mio sito in forma di forum, con l'aiuto di un amico che mi hostava questi esperimenti gratuitamente, e sognando una interazione con visitatori ed amici ai quali giravo il link dei nuovi articoli man mano che li scrivevo, qualche anno prima che i social esplodessero.

Una continua serie di problemi legati all'aggiornamento dei server e ai bachi di sicurezza di e107 richiedeva molta più dedizione di quella che ero disposto a mettere in campo, quindi dopo qualche anno abbandonai completamente il progetto e cancellai tutto.

## 2014: landing page (e dominio)

Parlando con un collega, mi suggerisce [Tophost](https://www.tophost.it) per registrarmi il nome di dominio e avere un minimo di spazio online a costi bassissimi.

Quindi decido di registrare il dominio raffaelebianco.it "per usi futuri", e di metterci dentro intanto una banale landing page simile alle migliaia che oggi si trovano fatte con [Linktr.ee](https://linktr.ee) e relativi cloni.

Per l'occasione studio e provo qualche tema gratuito in formato HTML5, approfondisco il CSS, scopro [Font Awesome](https://fontawesome.com) e alla fine ne esce la homepage che ancora oggi vedi quando visiti [www.RaffaeleBianco.it](https://www.RaffaeleBianco.it).

## 2015: Wordpress

Non ricordo come, ma mi sono imbattuto in Wordpress: l'idea di avere tutto online (l'editor WYSIWYG, i testi, le immagini) e tutto facilmente configurabile da qualunque dispositivo compreso lo smartphone mi aveva conquistato subito.

E allora ho creato il mio primo vero "blog", così da imparare a muovermi un po' anche in Wordpress.

In quella versione del sito ho trasportato alcune cose che avevo già pubblicato nella versione "e107", recuperandole da un backup, giusto per avere un minimo di contenuto con cui giocare, e ho continuato aggiungendo le cose che trovi anche qui, per la maggior parte video che pubblicavo su YouTube, fino ai contenuti del 2023 compresi.

## 2024: Hugo

Ed eccoci alla versione attuale, questa che stai guardando, fatta con [Hugo](https://gohugo.io).

Ho esportato tutto il contenuto da Wordpress su un file XML, ho usato [questo script](https://github.com/lonekorean/wordpress-export-to-markdown) per convertire l'XML in una struttura di file compatibile con Hugo, ho scelto un [tema per Hugo](https://themes.gohugo.io) che mi piaceva, un po' di studio online e di esperimenti la sera, e a meno di qualche dettaglio questa nuova versione del sito era già pronta e navigabile in locale sul mio PC dopo poche ore.

Questo tema ha le funzionalità più importanti che avevo anche in Wordpress (gestione di articoli, categorie, ricerca), ma risponde al mio desiderio di questi ultimi tempi di snellire le cose e tornare all'essenziale.

Hugo mi consente di:

- Sbarazzarmi completamente della pubblicità imposta su ogni blog free hostato su Wordpress.com.
  - Ci tenevo molto sia perché intralciano il lettore, sia perché la detesto in modo viscerale insieme a tutta la web economy basata sulla profilazione.
- Avere un sito web più reattivo.
  - Siamo nel 2024 e non è ammissibile dover *aspettare* per caricare una banale pagina web con testo e un paio di immagini.
- Poter editare i miei contenuti in locale, scrivendoli in Markdown dentro a VS Code, così guadagno anche l'integrazione con Git e tante altre funzionalità comode, ma potenzialmente anche con un qualunque editor di testo leggero che sul mio vetusto [IBM Thinkpad X60]({{< ref "pc-maggiorenne.md" >}}) sicuramente vanno meglio.
  - Scrivere in Markdown in un editor di testo, invece che in un editor [WYSIWYG](https://it.wikipedia.org/wiki/WYSIWYG), è un'esperienza molto particolare per quanto mi riguarda. E' forse difficile da capire finché non la si prova, ma il senso di "essenziale" veicolato dal testo a spaziatura fissa e dall'assenza completa di pulsanti e interfaccia grafica tiene l'occhio e la mente libera da distrazioni, e si scrive con più gusto, un po' come fosse una moderna macchina da scrivere invece di Word.

Buona navigazione.
