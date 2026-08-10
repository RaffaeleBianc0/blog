---
title: "Software free che uso (anche) sul PC aziendale"
description: "..."
date: "2026-07-01"
lastmod: '2026-08-08'
categories: 
  - "tecnologia"
image: "images/repoRefresh.png"
draft: "true"
---

A lavoro uso il notebook che mi è stato assegnato dall'azienda.
Questo mi ha portato a riflettere su un aspetto di cui non mi sono mai interessato granché: la licenza d'uso dei software che aggiungo io al PC. Ci sono alcuni programmi abbastanza noti nel panorama dei tool gratuiti, come PicPick e XnView, che usavo da anni anche su tutti i PC di lavoro che mi sono passati per le mani, senza che la rispettiva licenza d'uso me lo consentisse.

Il PC di lavoro inoltre è amministrato centralmente dall'IT, e questo significa che installare software è davvero scomodo per me utente non-amministratore.

I due punti che ho appena descritto mi hanno portato a cercare e trovare alcune soluzioni di cui voglio parlare in questo articolo:
- scoop
- software free utilizzabili anche a lavoro senza problemi di licenza

SCOOP
Questo tool da riga di comando serve a installare software nel profilo utente invece che a livello di sistema, quindi non servono i privilegi amministrativi.
Praticamente, a grandi linee, invece di installare un programma normalmente ne scarica una versione "portable", la estrae nella %USERPROFILE% in una sottocartella della cartella scoop\, e aggiunge al menu Start l'icona necessaria.
Tutto funziona quasi sempre come se l'app fosse stata installata col metodo tradizionale, ma con alcuni vantaggi interessanti, tra cui forse quello che preferisco è l'aggiornamento massivo di tutte le applicazioni installate tramite scoop. 
Non serve più fare la ricerca dei setup aggiornati nei vari siti dei produttori, download, doppioclick, avanti avanti avanti tra le opzioni, aspettare, cliccare fine, e ripetere tutto il giro per ciascun programma: basta scrivere "scoop update *" e fa tutto da solo, su tutte le applicazioni installate tramite scoop. La libreria di app supportate è davvero gigantesca, e ci sono molto probabilmente tutti i tool che usi quotidianamente. Ne ho poi scoperti un bel po' che non conoscevo, soprattutto piccoli tool da console.

VSCode
Questo è l'editor di testo che preferisco da quando è uscito, e di seguito voglio dettagliare le funzioni e le estensioni principali che mi servono a lavoro e che 
TODO
Estensioni: FlexLM, Rainbow CSV, Output Colorizer (per i log), REG, syslog-ng, TODO Highlight, vscode-util (?)
TODO

ShareX (sostituisce PicPick e fa più cose)
Salvare uno screenshot fa parte delle funzioni base del sistema operativo: in Win11, Win+Shift+S avvia lo Strumento di Cattura, che va bene per le esigenze di base, anche per registrare video.
Però appena ti serve fare "meglio" queste cose, ti accorgi che allo Strumento di Cattura mancano funzionalità: frecce, timbri, blur dei dati sensibili, eccetera.
Per anni ho risolto usando PicPick in versione free, che non è niente male, ma nel 2026 ho notato che la sua licenza d'uso non ne consente l'uso free per scopi business, e io a lavoro faccio davvero un sacco di screenshot.
Allora ho chiesto a Gemini quali alternative ci fossero gratuite anche per uso business, e mi ha restituito qualche nome, tra i quali ho ritrovato ShareX: avevo già visto questo software sul desktop di un cliente anni fa, e l'avevo anche provato per concludere un po' frettolosamente "troppo confusionario, troppe funzioni, resto su PicPick".
Beh, mi sbagliavo. E non solo sulla licenza (di cui al tempo non mi interessavo), ma anche sulla praticità e sulle features.
Cosa fa ShareX che PicPick non faceva? Evidenzia comodamente i bordi delle finestre così prendi la finestra intera con un click singolo, oppure fai il solito drag'n'drop per fare il riquadro grande quanto vuoi; puoi disegnare frecce vettoriali, le puoi curvare, puoi applicare timbri progressivi 1 2 3 4 che puntano dove vuoi con una freccia, puoi registrare video (sia mp4 con audio, sia gif animata). E queste sono più o meno le funzioni che uso regolarmente. 
Poi ce ne sono un botto che non sto usando, tra effetti, automatismi, e procedure varie: OCR, caricamento automatico online, eccetera.
Tutto questo ben di dio non intralcia l'uso "snello" che era un punto forte di PicPick, perché sono tutte voci di menu disponibili nell'iconcina nella tray, e le cerchi solo se ti servono. Sennò ti basta un click o un colpo di STAMP sulla tastiera, e fai il tuo screenshot.

nomacs (sostituisce XnView e l'imbarazzante app "Foto" di Windows)

TODO
