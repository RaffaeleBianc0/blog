---
title: "Il disco USB definitivo"
description: "ISO avviabili multiple, Windows To Go, rescue-disk, PortableApps, 2 Linux live superleggeri, storage veloce e criptato... serve altro?"
date: "2026-08-19"
lastmod: '2026-08-20'
categories: 
  - "tecnologia"
image: "images/golden.jpg"
draft: false
---

A forza di esperimenti con virtual machines, chiavette usb, smontaggio di computer e ISO avviabili, credo di essere finalmente arrivato a realizzare il mio **disco esterno definitivo**.  
Se come me sistemi PC (tuoi o altrui) di tanto in tanto, allora potrebbe interessarti quanto segue.

Come caratteristiche fisiche, la mia scelta è stata:
- ssd NVMe PCIe 4.0 per la **massima velocità** e **durata più elevata** rispetto alle normali chiavette, anche se un po' più ingombrante (diciamo che non posso più usare l'unità come portachiavi, ma in tasca ci sta ancora)
- box esterno in metallo, per la **massima resistenza meccanica** (che se lo porti in tasca può tornare utile) e **dissipazione del calore** che i dischi veloci producono in abbondanza sotto stress
- interfaccia e cavetto USB-C per le **massime prestazioni** e **compatibilità universale** (basta un adattatore da 2 euro per usarlo sulle vecchie porte USB-A)

Queste sono le funzionalità presenti:
- spazio di **storage**, ovviamente
- cartella **PortableApps** farcita di programmi che uso regolarmente sul PC, tutti in versione portable così da essere eseguiti ovunque senza doverli installare
- possibilità di fare il boot del computer da questo disco USB, e selezionare una di queste opzioni:
  - ISO di **installazione Win10+11+2022+2025**, aggiornate e soprattutto patchate in modo da saltare i requisiti di Win11, le fastidiose domande sulla profilazione, e l'obbligo di usare un account Microsoft: queste ISO servono sia per installare Windows da zero su un PC, sia per aggiornare una installazione esistente
  - ISO di un **rescue-disk** pieno di tool per provare a recuperare i dati da un PC che non si avvia
  - ISO di antiX e Puppy, 2 **distribuzioni Linux light** da usare/installare su PC molto vecchi
  - VHDX (disco virtuale) Windows To Go, cioè una **installazione portatile di Win10**, che mi è stata preziosa per far funzionare un vecchio dispositivo di acquisizione video incompatibile con Win11, senza costringermi a installare Win10 nel disco principale del PC

Se il disco è sufficientemente capiente, è possibile partizionarlo e criptare la partizione "storage" (per esempio con Bitlocker), così da aggiungere alle funzionalità elencate sopra anche la **cifratura dei dati archiviati**.

Credo che questo ventaglio copra tutte le esigenze che ho avuto usando dischi e chiavette usb negli ultimi 30+ anni.

Per realizzarlo, ci sono un po' di cose da procurare e da fare.

# Da procurare
- un disco NVMe esterno da almeno 128GB
  - Alternativa più versatile: disco NVMe + box usb-c
  - Alternativa più lenta ma più economica: disco SATA + box SATA
  - Alternativa più lenta ma più compatta: chiavetta usb veloce
- [Ventoy](https://www.ventoy.net), che consente il multi-boot da qualsiasi file ISO/VHDX presente nel disco
- [Rufus](https://rufus.ie): servirà per creare l'installazione Windows To Go
- [PortableApps.com](https://portableapps.com) + la tua selezione di app (facilmente scaricabili dall'interfaccia del PortableApps Launcher)
- ISO rescue-disk (es. [Hiren's BootCD](https://www.hirensbootcd.org), ma ce ne sono vari online)
- ISO di installazione Windows (scaricabili per es. da [UUP dump](https://uupdump.net/) oppure da [massgrave.dev](https://massgrave.dev/genuine-installation-media))
- ISO bootable a piacere (es. distribuzioni Linux, io ci ho messo [Puppy](https://puppylinux-woof-ce.github.io/) e [antiX](https://antixlinux.com/) perché mi capita di usare Linux quasi sempre per resuscitare PC obsoleti, e più leggere sono meglio è)



# Procedura
Intanto scrivo i passaggi come me li sono appuntati; poi un giorno se ne avrò voglia aggiungerò dettagli e screenshot.

1. Attivare Hyper-V in Windows (se hai Windows Home, allora cerca online la procedura tramite Powershell)  

1. Installare Ventoy nell'SSD esterno, usando le opzioni NTFS e GPT.  

1. SSD > Creare la cartella \ventoy e copiarci dentro il plugin per leggere i dischi VHD/VHDX (si trova sul sito di Ventoy).  

1. <kbd>Win</kbd>+<kbd>X</kbd> > Gestione disco > Creare un VHDX dinamico da almeno 50GB formattato in NTFS, e inizializzarlo.  

1. Rufus > installare Windows To Go nel disco VHDX (c'è l'opzione dedicata, supporta sia Win10 che Win11).  

1. <kbd>Win</kbd>+<kbd>X</kbd> > Gestione disco > Smontare il VHDX.  

1. Hyper-V > nuova VM, che monti il file VHDX come disco, e avviarla > completare la procedura di primo avvio Windows, opzionalmente installare i software che servono nell'ambiente Windows To Go, e chiudere la sessione arrestando Windows e attendendo che la VM si spenga regolarmente.  

1. Copiare il VHDX nell'SSD Ventoy, insieme ad eventuali altri file ISO.  
