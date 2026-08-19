---
title: "Software free che uso (anche) sul PC aziendale"
description: "... rispettando licenze d'uso e privilegi utente limitati"
date: "2026-07-01"
lastmod: '2026-08-08'
categories: 
  - "tecnologia"
image: "images/software.jpg"
draft: true
---

A lavoro uso il notebook che mi è stato assegnato dall'azienda, e questo utilizzo è soggetto a policy ufficiali che valgono per tutti i dipendenti.  
Questo mi ha portato a riflettere su un aspetto di cui non mi sono mai interessato granché: la **licenza d'uso dei software che aggiungo io** al PC.  
Ci sono alcuni programmi abbastanza noti nel panorama dei tool gratuiti, come PicPick e XnView, che usavo da anni anche su tutti i PC di lavoro che mi sono passati per le mani, senza che la rispettiva licenza d'uso me lo consentisse.

Il PC di lavoro inoltre è **amministrato centralmente dall'IT**, e questo significa che installare software è davvero scomodo per me utente non-amministratore.

I due punti che ho appena descritto mi hanno portato a cercare e trovare alcune soluzioni di cui voglio parlare in questo articolo:
- scoop
- software free utilizzabili anche a lavoro senza problemi di licenza

# scoop
Questo tool da riga di comando serve a installare software nel profilo utente invece che a livello di sistema, quindi non servono i privilegi amministrativi.  
Attenzione: il fatto che sia un tool da CLI rende le installazioni molto più **facili** di quanto si faccia normalmente con Windows, avvicinandole alla praticità e immediatezza offerte dai package manager in Linux.

Praticamente, a grandi linee, invece di installare un programma normalmente, ne scarica una versione "portable", la estrae in `%USERPROFILE%\scoop\<nomeapp>`, e aggiunge al menu Start l'icona necessaria.
Tutto funziona come se l'app fosse stata installata col metodo tradizionale, ma con alcuni vantaggi interessanti, tra cui forse quello che preferisco è l'aggiornamento massivo di tutte le applicazioni installate tramite scoop: non devo più fare la ricerca dei setup aggiornati nei vari siti dei produttori, download, doppioclick, avanti avanti avanti tra le opzioni, aspettare, cliccare fine, e ripetere tutto il giro per ciascun programma: mi basta scrivere `scoop update *` e fa tutto da solo, su tutte le applicazioni installate tramite scoop.  
La libreria di app supportate è davvero gigantesca, e ci sono molto probabilmente tutti i tool che usi quotidianamente.  
Ne ho poi scoperti un bel po' che non conoscevo, soprattutto piccoli tool da console davvero potenti.

# App
Di seguito faccio un rapido cenno alle app free anche per uso business alle quali non posso più rinunciare.

## VSCode
Questo è l'editor di testo che preferisco da quando è uscito.  
Un po' pesante, ma le funzioni che offre compensano ampiamente il mezzo secondo in più che ci mette ad avviarsi (il che accade una volta alla settimana, perché ce l'ho costantemente aperto).  
Vedo che i colleghi sono affezionati a [Notepad++](https://notepad-plus-plus.org/), programma eccellente e a volte indispensabile per aprire file giganteschi; ma la comodità di VSCode è ampiamente superiore.  

Queste sono le estensioni principali che mi sono utilissime nel lavoro che faccio (le trovi tutte con la ricerca integrata in VSCode):

1. **Rainbow CSV**: la salvezza per lavorare con i CSV, perché colora le colonne e consente di visualizzarle allineate verticalmente

1. **Bookmarks**: una scorciatoia per mettere/togliere un segnalibro nella riga corrente, un'altra scorciatoia per andare al prossimo segnalibro. Essenziale in tutti i sensi.

1. **TODO Highlight**: evidenzia e raccoglie tutti i TODO e i FIXME inseriti nei file di testo (tipicamente codice sorgente), così da ritrovarli con un click.

1. **XML Tools**: formatta correttamente file XML, e consente di navigare l'XML tramite un tree

1. **Output Colorizer**: colorazione della sintassi per i file LOG (molto usati dal prodotto di cui mi occupo)

1. **syslog-ng**: colorazione della sintassi per i file .syslog (molto usati dal prodotto di cui mi occupo)

1. **FlexLM**: colorazione della sintassi per i file di licenza FlexLM (usati dal prodotto di cui mi occupo)

1. **REG**: colorazione della sintassi per i file REG (Windows Registry)




## ShareX (sostituisce PicPick e fa più cose)
Salvare uno screenshot fa parte delle funzioni base del sistema operativo: in Win11, Win+Shift+S avvia lo Strumento di Cattura, che va bene per le esigenze di base, anche per registrare video.
Però appena ti serve fare "meglio" queste cose, ti accorgi che allo Strumento di Cattura mancano funzionalità: frecce, timbri, blur dei dati sensibili, eccetera.
Per anni ho risolto usando PicPick in versione free, che non è niente male, ma nel 2026 ho notato che la sua licenza d'uso non ne consente l'uso free per scopi business, e io a lavoro faccio davvero un sacco di screenshot.
Allora ho chiesto a Gemini quali alternative ci fossero gratuite anche per uso business, e mi ha restituito qualche nome, tra i quali ho ritrovato ShareX: avevo già visto questo software sul desktop di un cliente anni fa, e l'avevo anche provato per concludere un po' frettolosamente "troppo confusionario, troppe funzioni, resto su PicPick".
Beh, mi sbagliavo. E non solo sulla licenza (di cui al tempo non mi interessavo), ma anche sulla praticità e sulle features.
Cosa fa ShareX che PicPick non faceva? Evidenzia comodamente i bordi delle finestre così prendi la finestra intera con un click singolo, oppure fai il solito drag'n'drop per fare il riquadro grande quanto vuoi; puoi disegnare frecce vettoriali, le puoi curvare, puoi applicare timbri progressivi 1 2 3 4 che puntano dove vuoi con una freccia, puoi registrare video (sia mp4 con audio, sia gif animata). E queste sono più o meno le funzioni che uso regolarmente. 
Poi ce ne sono un botto che non sto usando, tra effetti, automatismi, e procedure varie: OCR, caricamento automatico online, eccetera.
Tutto questo ben di dio non intralcia l'uso "snello" che era un punto forte di PicPick, perché sono tutte voci di menu disponibili nell'iconcina nella tray, e le cerchi solo se ti servono. Sennò ti basta un click o un colpo di STAMP sulla tastiera, e fai il tuo screenshot.

## nomacs (sostituisce XnView e l'imbarazzante app "Foto" di Windows)
TODO
