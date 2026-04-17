---
title: "Hugo"
description: "No, non l'aperitivo altoatesino"
date: "2024-02-09"
lastmod: '2025-11-22'
categories: 
  - "tecnologia"
image: "images/hugo-logo.png"
---

In questo post ti racconto della ristrutturazione di questo blog nella forma attuale.



# Cosa e quando

Fino al 2024 questo blog era hostato su [Wordpress.com](http://Wordpress.com), ne parlo nella [storia di questo sito](/blog/p/storia-di-questo-sito-web/#2015-blog-su-wordpress).

A inizio 2024 ho scoperto dell'esistenza degli [SSG](https://en.wikipedia.org/wiki/Static_site_generator) (_Static Site Generators_), software che trasformano contenuti scritti in [Markdown](https://en.wikipedia.org/wiki/Markdown) in siti web veloci e con le funzionalità che servono ad un blog.  
E io che pensavo che i siti web statici fossero praticamente spariti dall'avvento del Web 2.0 dei primi anni 2000!

Ci ho messo un po' di giorni a capire quale dei tanti SSG esistenti fosse quello su cui puntare, cioè quello aggiornato recentemente e regolarmente, e con una user-base la più estesa possibile per chiedere aiuto nel caso servisse.  

Ha vinto [Hugo](https://gohugo.io).

Lo ho scaricato (è un singolo eseguibile portable), ho subito provato a creare un micro-sito di prova in locale, ci ho messo meno di quanto pensassi e mi è piaciuto.



# Perché

Ho trasformato il mio blog da Wordpress a Hugo per questi motivi.



## Pubblicità

Prima di tutto, **sbarazzarmi della pubblicità**.

**L'economia dell'attenzione, con la pubblicità ovunque e la profilazione costante, mi sono diventate intollerabili**, quindi liberarmi di tutto questo almeno nelle _mie_ pagine è stato il motivo numero 1 per la transizione a Hugo. Quasi una scelta etica.

Questo è un piccolo blog, e non mi serve chissà quale servizio per ospitarlo, basta il minimo, e il minimo quando si tratta di Wordpress significa Wordpress.com, che per offrire il suo servizio gratuito infarcisce di stramaledetta pubblicità ogni pagina di quello che scrivi.



## Performance

Il motivo numero 2 sono le performance: **le pagine statiche generate da Hugo si caricano in un istante**, e va tutto veloce.  
Wordpress invece, che è un sistema super articolato per gestire siti dinamici, ad ogni click va ad interrogare un database e a costruire la pagina dinamicamente, e ci mette del tempo, lo senti quando fai click, e dopo tre click sei già nervosetto.  

Io ho un semplice blog, i contenuti li pubblico solo io e sono statici, cioè non cambiano fino alla prossima pubblicazione, quindi non mi serve un database sotto né potenza di elaborazione lato hosting per generare le pagine da zero ogni volta che il lettore clicca un link.  
Il 1996 è passato da un pezzo, oggi non è ammissibile dover *aspettare* per caricare una banale pagina web con testo e un paio di immagini.



## Sicurezza

Per risolvere il problema della pubblicità avrei potuto semplicemente installare Wordpress nel mio hosting.  
Ma non volevo cadere di nuovo nella [trappola sistemistica che ho già vissuto anni fa con i CMS]({{< ref "storia-del-sito.md#2005-cms" >}}): voglio solo pubblicare quello che scrivo, senza star dietro ai problemi di sicurezza di un database mysql, o dei plugin di Wordpress.

La scelta più sicura è sbarazzarsi di quelle dipendenze, e un sito statico mi sembra l'opzione più centrata per ottenere questo risultato.



## Markdown

Poi avevo voglia di editare i miei contenuti in locale, scrivendoli in Markdown dentro a [VS Code](https://code.visualstudio.com), con la sua ottima integrazione con [GitHub](https://github.com/RaffaeleBianc0), ma potenzialmente anche con un qualunque editor di testo leggero da usare nel mio vetusto [IBM Thinkpad X60]({{< ref "pc-maggiorenne.md" >}}).

**Scrivere in Markdown usando un editor di testo**, invece che scrivere direttamente in un editor [WYSIWYG](https://it.wikipedia.org/wiki/WYSIWYG) come quello di Wordpress, è un'esperienza particolare.  
L'editor di testo, senza troppi pulsanti e menu, con la font a spaziatura fissa, senza automatismi, correzioni automatiche, stili, e tutte le altre cose che fanno parte della moderna stesura di testi al computer, è un po' come **la versione moderna della macchina da scrivere**: tiene l'occhio e la mente libera da distrazioni, e finisce che **scrivo con più gusto**.

Il Markdown lo stavo già usando da un bel po', sia per rendere un po' più strutturati i piccoli file di testo sparsi ovunque quando si lavora con i computer, sia soprattutto nell'uso quotidiano di [Obsidian](http://obsidian.md) che accompagna la mia vita lavorativa degli ultimi anni.



## Imparare

Come ultima motivazione ci metto la voglia di imparare i rudimenti di Hugo di per sé, come tecnologia e approccio diversi per pubblicare contenuti.



# Come

Per passare da Wordpress allo stato attuale del blog, ho fatto un po' di lavoro.



## Export e conversione

Prima di tutto ho **esportato tutto il contenuto da Wordpress su un file XML**, c'è il comando nella dashboard di amministrazione.

Poi ho usato [questo script](https://github.com/lonekorean/wordpress-export-to-markdown) per **convertire l'XML in una struttura di file Markdown compatibile con Hugo**.  
Lo script si è preoccupato anche di fare il download delle immagini dal mio blog Wordpress, posizionandole in modo ordinato e linkandole correttamente nei file Markdown generati.



## Tema 

Ho scelto un [tema per Hugo](https://themes.gohugo.io) che mi piaceva ([Stack](https://github.com/CaiJimmy/hugo-theme-stack)), perché ha una estetica ariosa che mi comunica semplicità, e una serie di caratteristiche e di funzionalità che cercavo:

* **colonne fisse ai lati**, nella versione desktop (menu a sinistra, e widget a destra: quasi tutti i display dei PC sono 16:9, e tutto quello spazio ai lati del testo _deve_ essere utilizzato, dal mio punto di vista)
* **layout responsive**, che su schermi più piccoli toglie i widget e sposta menu e ToC su pulsanti poco invasivi
* **categorie** personalizzabili (supporta anche i **tag**, ma non li uso per mantenere tutto più snello)
* **ToC** (Table of Contents) con evidenziatura dinamica del paragrafo visualizzato
* **ricerca** sui contenuti dell'intero blog

... ed alcune che non mi aspettavo ma che ho apprezzato:

* **gestione immagini** automatica (resize e carosello) 
* **light/dark mode** (a me piace dark, ma magari sotto all'ombrellone in spiaggia si legge meglio light)
* **feed RSS** automatico (qualcuno li usa ancora?)

Un po' di studio online e di esperimenti la sera, e a meno di qualche dettaglio questa nuova versione del sito era già pronta e navigabile in locale sul mio PC dopo poche ore.



## Deploy 

Per pubblicare il blog compilato con Hugo, inizialmente ho fatto il banale upload nel mio spazio FTP come facevo 30 anni fa, ma ho scoperto presto due approcci più raffinati.

Per primo [**Rclone**](http://rclone.org), un potente tool da linea di comando per sincronizzare file e cartelle con le destinazioni più diverse, tra cui anche un normale spazio FTP come nel mio caso.  

Dopo poco tempo però scopro il metodo che sto usando adesso, che aggiunge a tutto il workflow qualche feature che credevo di aver perso abbandonando Wordpress:

1. Modifico i miei file Markdown in locale usando VS Code, che è già il mio editor di testo preferito praticamente da quando è stato rilasciato nel 2015.  

1. Con l'integrazione GitHub installata in VS Code, con un click faccio l'**upload dei file nuovi e modificati nel mio repository privato su GitHub**, che significa ottenere in automatico questi vantaggi:
    * **backup** online di tutti i file sorgente del blog
    * **versionamento** di ogni file (posso tornare indietro nella storia se qualcosa non mi piace o si rompe)
    * **editor VS Code online** per modificare i miei file da qualunque computer e aggiornare così il blog anche quando non ho il mio PC, basta premere il punto {{< tasto "." >}} sulla tastiera mentre stai visualizzando un file. Spettacolo!  

1. Una [**GitHub Action**](https://github.com/features/actions) fa la magia ogni volta che il mio repository "sente" una modifica, e automaticamente fa queste cose in background in un paio di minuti:
    * installa l'ultima versione di Hugo in una VM di GitHub
    * ricompila in quella VM il blog
    * dei file ottenuti, fa l'upload sul mio FTP solo di quelli aggiunti e modificati (questo modulo ogni tanto dà errore, ma amen, di solito al prossimo sync funziona)  

Sì, adoro quando i computer lavorano per me.

Questa è la GitHub Action, se può tornare utile:

```YAML
name: Hugo Build and FTP Deploy
on:
  push:
    branches:
      - main
jobs:
  deploy:
    runs-on: ubuntu-latest
    
    steps:
      - name: Checkout repository
        uses: actions/checkout@v4
        with:
          submodules: true
          fetch-depth: 0
      - name: Setup Hugo
        uses: peaceiris/actions-hugo@v2
        with:
          hugo-version: 'latest'
          extended: true
      - name: Build
        run: hugo --minify
      - name: FTP Deploy
        uses: SamKirkland/FTP-Deploy-Action@v4.3.6
        with:
          server: ${{ secrets.FTP_SERVER }}
          username: ${{ secrets.FTP_USERNAME }}
          password: ${{ secrets.FTP_PASSWORD }}
          local-dir: ./public/
          server-dir: ./blog/
          timeout: 120000
```



## Hack

Cercando il modo di avere la ToC anche nella versione mobile del blog (che di default è assente nel tema Stack), ho poi trovato alcune informazioni per applicare sia quella che altre modifiche interessanti al tema, su [MomentoDiMezzo.com](https://momentodimezzo.com/en/p/blog-customization) e su [LucasLifes.com](https://blog.lucaslifes.com/categories/hugo-blog/).

Mi sono anche fatto aiutare parecchio da **Copilot integrato in VS Code** per fare alcune modifiche minori che, senza una AI di supporto, non sarei mai stato capace di fare in tempi ragionevoli - ad esempio l'evidenziatura completa dei link al passaggio del mouse nel corpo del testo e nella ToC.  
Per inciso, vedere come l'AI ha analizzato l'intero progetto Hugo e ha applicato le modifiche dove necessario, tutto direttamente in VS Code, mi ha lasciato senza parole.



# Godo

Insomma ho scavalcato i limiti di Wordpress e posso dire che **oggi le funzionalità e l'estetica di questo blog sono proprio quelle che volevo**.  

Anche il viaggio per arrivare qui è stato molto stimolante, perché ho conosciuto e usato qualche strumento che prima avevo solo sentito nominare (Hugo, GitHub, Rclone, Copilot in VS Code).
