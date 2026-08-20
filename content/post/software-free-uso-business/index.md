---
title: "Software free che uso (anche) sul PC aziendale"
description: "... rispettando licenze d'uso e privilegi utente limitati"
date: "2026-08-20"
lastmod: "2026-08-20"
categories: 
  - "tecnologia"
image: "images/software.jpg"
draft: false
---

A lavoro uso il notebook che mi è stato assegnato dall'azienda, e questo utilizzo è soggetto a policy che valgono per tutti i dipendenti.  
Questo mi ha portato a riflettere su un aspetto di cui non mi sono mai interessato granché: la **licenza d'uso dei software che scelgo di utilizzare** su questo PC.  
Per esempio ci sono alcuni programmi abbastanza noti nel panorama dei tool gratuiti, come PicPick e XnView, che usavo da anni anche su tutti i PC di lavoro che mi sono passati per le mani, senza che la rispettiva licenza d'uso me lo consentisse.

Il PC di lavoro inoltre è **amministrato centralmente dal reparto IT**, e questo significa che installare software aggiuntivo è davvero scomodo per me utente non-amministratore, o addirittura impossibile.

I due punti che ho appena descritto mi hanno portato a cercare e trovare alcune soluzioni di cui voglio parlare in questo articolo:
- scoop
- software free utilizzabili anche a lavoro

# scoop
Questo tool da riga di comando (CLI) serve a installare software nel profilo utente invece che a livello di sistema, quindi non servono i privilegi amministrativi.  
Attenzione: il fatto che sia un tool CLI rende le installazioni molto più **facili** di quanto lo siano normalmente con Windows, avvicinandole alla praticità e immediatezza offerte dai package manager in Linux.

Praticamente, a grandi linee, invece di installare un programma normalmente, scoop ne scarica una versione "portable", la estrae in `%USERPROFILE%\scoop\<nomeapp>`, e aggiunge al menu Start dell'utente l'icona necessaria ad avviarlo.
Tutto funziona come se l'app fosse stata installata col metodo tradizionale, ma con alcuni vantaggi interessanti, tra cui forse quello che preferisco è l'aggiornamento massivo di tutte le applicazioni installate tramite scoop con un singolo comando elementare: `scoop update *` e fa tutto da solo.  
La libreria di app supportate è davvero gigantesca, e ci sono molto probabilmente tutti i programmi che usi quotidianamente.  
Ne ho poi scoperti un bel po' che non conoscevo, soprattutto piccoli tool da console davvero ben fatti (fzf, ov, btop++, gping, powerping, bat, zoxide, ...), che spingono ad usare di più il terminale rispetto a mouse e finestre, e di conseguenza ad essere più veloci in generale a fare le cose (eh già, la cara vecchia tastiera in molti contesti batte il mouse a mani basse, non va confusa la facilità con la velocità).

# Applicazioni free
Di seguito faccio un rapido cenno alle app free anche per uso business alle quali non voglio più rinunciare.

## 7-Zip
**Sostituisce:** WinZip, WinRAR, Cartelle compresse di Windows  
**Website:** https://www.7-zip.org  
**scoop:** `scoop install 7zip`

Programma essenziale nella sua estetica ancorata ai primi anni 2000, e perciò veloce ed efficace.  
Il supporto al formato .7z è stato aggiunto in Win11, ma la praticità dell'originale 7-Zip per creare ed estrarre archivi tutto da menu contestuale di Explorer resta finora imbattuta.

## VSCode
**Sostituisce:** Blocco note, Notepad++  
**Website:** https://code.visualstudio.com/  
**scoop:** `scoop install vscode`

Questo è l'editor di testo che preferisco da quando è uscito.  
È un po' pesante, ma le funzioni che offre compensano ampiamente il mezzo secondo in più che ci mette ad avviarsi (il che accade una volta alla settimana, perché ce l'ho costantemente aperto).  
Vedo molti colleghi affezionati a [Notepad++](https://notepad-plus-plus.org/), programma eccellente che usavo prima di VSCode, e che a volte mi torna ancora utile per aprire file giganteschi (es. alcuni log "maturati" per mesi); ma la comodità e la potenza di VSCode per l'uso quotidiano sono secondo me superiori.  

Queste sono le estensioni principali che mi sono utilissime nel lavoro che faccio (le trovi tutte con la ricerca integrata nel pannello delle estensioni di VSCode, <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>X</kbd>):

1. **Rainbow CSV**: fondamentale per lavorare con i CSV, perché colora le colonne, consente di visualizzarle allineate verticalmente, consente di verificare la struttura del CSV e di interrogarlo con delle query in simil-SQL.

1. **Bookmarks**: una scorciatoia da tastiera per mettere/togliere un segnalibro nella riga corrente, un'altra scorciatoia per andare al prossimo segnalibro. Essenziale, in tutti i sensi.

1. **TODO Highlight**: evidenzia e raccoglie tutti i TODO e i FIXME inseriti nei file di testo di un intero progetto (tipicamente codice sorgente), così da ritrovarli con un click.

1. **XML Tools**: formatta correttamente file XML, e consente di navigare l'XML tramite un tree

1. **Output Colorizer**: colorazione della sintassi per i file LOG (molto usati dal prodotto di cui mi occupo)

1. **syslog-ng**: colorazione della sintassi per i file .syslog (molto usati dal prodotto di cui mi occupo)

1. **FlexLM**: colorazione della sintassi per i file di licenza FlexLM (usati dal prodotto di cui mi occupo)

1. **REG**: colorazione della sintassi per i file REG (Windows Registry)




## ShareX
**Sostituisce:** Strumento di cattura, PicPick  
**Website:** https://getsharex.com  
**scoop:** `scoop install sharex`

Salvare uno screenshot fa parte delle funzioni del sistema operativo: in Win11, <kbd>Win</kbd>+<kbd>Shift</kbd>+<kbd>S</kbd> avvia la app "Strumento di cattura", che va bene per le esigenze di base, anche per registrare brevi video.

Però appena ti serve fare "meglio" queste cose, ti accorgi che allo Strumento di cattura mancano tante funzionalità.  
Per anni ho risolto usando PicPick in versione free, che non è niente male, ma recentemente ho verificato che la sua licenza d'uso non ne consente l'uso free per scopi business, e io a lavoro faccio davvero un sacco di screenshot.

Qualche ricerca, qualche prova veloce, ed ecco la mia soluzione: **ShareX**.  
Highlights:
- evidenzia i bordi delle finestre al passaggio del mouse, così catturi la finestra intera con un click singolo, oppure fai il classico drag'n'drop per fare il riquadro grande quanto vuoi
- puoi disegnare frecce vettoriali e curvarle (Bézier)
- puoi applicare timbri progressivi 1 2 3 4 che puntano dove vuoi con una freccia, eccellente per dare istruzioni su quali click fare in sequenza
- puoi registrare video, sia mp4 con audio, sia gif animate, ottime per documentare brevi passaggi

Poi ci sono una quantità di altre funzioni che non sto usando, tra effetti, automatismi, e procedure varie: OCR, caricamento automatico online, eccetera.  

Tutto questo ben di dio non intralcia l'uso "snello" che era un punto forte di PicPick, perché sono tutti comandi disponibili nell'iconcina nella tray che vai a cercare solo se ti servono, ma per l'uso quotidiano ti basta un click sulla stessa iconcina o un colpo di STAMP sulla tastiera, e fai il tuo screenshot.

## nomacs
**Sostituisce:** app "Foto" e "Microsoft Designer" di Windows, XnView, IrfanView  
**Website:** https://nomacs.org  
**scoop:** `scoop install nomacs`

Velocissimo visualizzatore di immagini.  
Già questo basta a farmelo preferire alla app di default "Foto" distribuita con Windows, che è lenta in modo imbarazzante.  
Stesso discorso per le possibilità di modifica delle immagini, nettamente superiori a quelle del default "Microsoft Designer" sempre distribuito con Win11.
