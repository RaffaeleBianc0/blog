---
title: "Hugo"
date: "2024-02-09"
lastmod: '2025-11-15'
categories: 
  - "tecnologia"
image: "images/hugo-logo.png"
---

Ti parlo di come è fatto questo blog, un po' dietro le quinte.

# Cosa e quando

Fino al 2024 questo blog era hostato su Wordpress.com, se vuoi ho scritto una paginetta anche sulla [storia di questo sito](/blog/p/storia-di-questo-sito-web) dove ne parlo.

A inizio 2024 ho scoperto gli [SSG](https://en.wikipedia.org/wiki/Static_site_generator), una categoria di software che consentono di trasformare contenuti scritti in [Markdown](https://en.wikipedia.org/wiki/Markdown) in siti web veloci e con tutte le funzionalità che servono. 

Ci ho messo un po' di giorni a capire quale, dei tanti SSG esistenti, fosse quello su cui puntare, cioè quello aggiornato recentemente, regolarmente, e con una user-base la più estesa possibile, per chiedere aiuto nel caso servisse. Ha vinto [Hugo](https://gohugo.io).

In uno dei miei periodici guizzi di nerdismo, ho subito provato a creare un micro-sito di prova in locale, ci ho messo meno di quanto pensassi e mi è piaciuto.

# Perché

Ho trasformato il mio blog da Wordpress a Hugo per questi motivi.

## Pubblicità

Prima di tutto, sbarazzarmi della pubblicità.

Questo è un piccolo blog, e non mi serve chissà quale servizio per ospitarlo, basta il minimo, e il minimo quando si tratta di Wordpress significa Wordpress.com, che per offrire il suo servizio gratuito infarcisce di stramaledetta pubblicità ogni pagina di quello che scrivi.

Ora, sarà la vecchiaia non lo so, ma la data economy basata sulla profilazione degli utenti a me sta dando sempre più fastidio, quindi liberarmi di questa cosa è stato il motivo numero 1 per la transizione a Hugo.

## Performance

Il motivo numero 2 sono le performance: le pagine statiche generate da Hugo si caricano in un istante, e va tutto veloce. Wordpress invece, che è un sistema super articolato per gestire siti dinamici, ad ogni click va ad interrogare un database e a costruire la pagina dinamicamente, e ci mette del tempo, lo senti quando fai click, e dopo tre click lo odi. Io ho un semplice blog, i contenuti sono quelli che pubblico e sono statici, cioè non cambiano fino alla prossima pubblicazione, non mi serve un database sotto né potenza di elaborazione lato hosting per generare le pagine da zero ogni volta che il lettore clicca un link. Il 1996 è passato da un pezzo, oggi non è ammissibile dover *aspettare* per caricare una banale pagina web con testo e un paio di immagini.

## Markdown

Motivo 3: poter editare i miei contenuti in locale, scrivendoli in Markdown dentro a [VS Code](https://code.visualstudio.com), con la sua strepitosa integrazione con [GitHub](https://github.com/RaffaeleBianc0) e tante altre funzionalità comode, ma potenzialmente anche con un qualunque editor di testo leggero che sul mio vetusto [IBM Thinkpad X60]({{< ref "pc-maggiorenne.md" >}}) sicuramente vanno meglio.

Scrivere in Markdown usando un editor di testo, invece che scrivere direttamente nell'editor [WYSIWYG](https://it.wikipedia.org/wiki/WYSIWYG) di Wordpress, è un'esperienza molto particolare per quanto mi riguarda. E' forse difficile da capire finché non la si prova, ma il senso di "essenziale" veicolato dal testo a spaziatura fissa e dall'assenza completa di pulsanti e interfaccia grafica tiene l'occhio e la mente libera da distrazioni, e si scrive con più gusto, un po' come fosse una moderna macchina da scrivere invece di Word, per fare un parallelo.

Il Markdown lo stavo già usando da un bel po', sia per rendere un po' più ricchi e strutturati i piccoli file di testo sparsi ovunque quando si lavora con i computer, sia soprattutto nell'uso quotidiano di [Obsidian](https://obsidian.md) che accompagna la mia vita lavorativa degli ultimi anni.

## Imparare

Al quarto posto come motivo ci metto la voglia di imparare i rudimenti di Hugo di per sé, come tecnologia e approccio diversi per scrivere post nel mio spazio web.

# Come

## Export e conversione

Per passare da Wordpress allo stato attuale del blog, ho fatto un certo lavoro.

Prima di tutto ho esportato tutto il contenuto da Wordpress su un file XML, c'è il comando nella dashboard di amministrazione.

Poi ho usato [questo script](https://github.com/lonekorean/wordpress-export-to-markdown) per convertire l'XML in una struttura di file compatibile con Hugo. Lo script si è preoccupato anche di fare il download delle immagini dal mio blog Wordpress.

## Tema 

Ho scelto un [tema per Hugo](https://themes.gohugo.io) che mi piaceva ([Stack](https://github.com/CaiJimmy/hugo-theme-stack)), perché ha le funzionalità più importanti che non volevo perdere (gestione di articoli, categorie, ricerca), e risponde al mio desiderio di questi ultimi tempi di snellire le cose e tendere un po' di più all'essenziale.

Un po' di studio online e di esperimenti la sera, e a meno di qualche dettaglio questa nuova versione del sito era già pronta e navigabile in locale sul mio PC dopo poche ore.

## Deploy 

Per pubblicare il blog compilato con Hugo inizialmente ho fatto il banale upload nel mio spazio FTP, ma ho scoperto presto due approcci progressivamente più nerd, che ovviamente mi hanno stuzzicato subito: prima [Rclone](https://rclone.org), che ho subito pilotato con un piccolo script per avere un deploy one-click dei soli file modificati, e poi il metodo che sto usando adesso, cioè una [GitHub Action](https://github.com/features/actions) che, ogni volta che faccio il push delle modifiche sul mio repository GitHub, in automatico ricompila il sito con Hugo e fa l'upload dei file cambiati sul mio FTP. In questo modo, creare e modificare i miei post si risolve in un click su un comando in VS Code, e a tutto il resto pensa GitHub.
Sì, adoro quando i computer lavorano per me.

## Hack

Cercando informazioni su come avere la ToC anche nella versione mobile del blog (che di default è assente nel tema Stack), ho poi trovato alcune informazioni per applicare quella e altre modifiche interessanti al tema, su [MomentoDiMezzo.com](https://momentodimezzo.com/en/p/blog-customization) e su [LucasLifes.com](https://blog.lucaslifes.com/p/hugo-stack-theme-customization).

Infine mi sono fatto aiutare da Copilot integrato in VS Code per fare alcune modifiche minori in pochi minuti che, senza una AI di supporto, non sarei mai stato capace di fare in tempi ragionevoli - ad esempio l'evidenziatura completa dei link al passaggio del mouse nel corpo del testo e nella ToC, ma non in altri punti. Per inciso, vedere come l'AI ha analizzato l'intero progetto Hugo e ha applicato le modifiche dove necessario, tutto direttamente in VS Code, mi ha lasciato senza parole.

# Conclusione

Le funzionalità di questo blog non sono ancora precisamente come le vorrei, ma direi che ci siamo al 90%, sono molto più soddisfatto di questa forma del blog rispetto alla precedente su Wordpress!
