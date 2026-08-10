---
title: "Il disco USB definitivo"
description: "..."
date: "2026-08-01"
lastmod: '2026-08-08'
categories: 
  - "tecnologia"
image: "images/disco-usb.png"
draft: true
---

A forza di esperimenti con virtual machines, chiavette usb, dischi esterni e ISO avviabili, credo di essere finalmente arrivato al disco esterno definitivo.
Se come me sistemi PC di tanto in tanto, allora potrebbe interessarti quanto segue.

Queste sono le caratteristiche:
- ssd nvme, notevolmente più veloce e più duraturo di una normale chiavetta, anche se un po' più ingombrante
- interfaccia USB-C per le massime prestazioni e compatibilità universale (basta un adattatore da 2 euro per usarlo sulle vecchie porte USB-A)
Queste sono le funzionalità presenti:
- spazio di storage, ovviamente
- cartella PortableApps farcita di programmi che uso regolarmente sul PC, tutti in versione portable così da essere eseguiti direttamente senza doverli installare
- possibilità di fare il boot del computer da questo disco USB, e selezionare una di queste possibilità:
  - ISO di installazione Win10+11+2022+2025, aggiornate e soprattutto patchate in modo da saltare i requisiti di Win11, le fastidiose domande sulla profilazione, e l'obbligo di usare un account Microsoft: queste ISO servono sia per installare Windows da zero su un PC, sia per aggiornare una installazione esistente
  - ISO di un rescue-disk pieno di tool per riuscire a recuperare i dati da un PC che non si avvia
  - ISO di antiX e Puppy, 2 distribuzioni Linux light da usare/installare su PC molto vecchi
  - VHDX (disco virtuale) Windows To Go, cioè una installazione portatile di Win10, che mi è stata preziosa per far funzionare un vecchio dispositivo di acquisizione video incompatibile con Win11, senza costringermi a installare Win10 nel disco principale del mio PC
Se il disco è sufficientemente capiente, è possibile partizionarlo e criptare la partizione "storage" (per esempio con Bitlocker), così da aggiungere alle funzionalità elencate sopra anche la crittografia dei dati archiviati.
Credo che questo ventaglio copra tutte le esigenze che ho avuto usando dischi e chiavette usb negli ultimi 30+ anni.

Per realizzarlo, ci sono un po' di cose da procurare e da fare.

# COSE DA PROCURARE
- un disco nvme esterno da almeno 128GB (alternative: disco nvme + box usb-c, disco SATA + box SATA, chiavetta usb veloce)
- Ventoy
- Rufus
- PortableApps.com
- ISO rescue-disk
- ISO di installazione Windows
- ISO bootable a piacere (es. distribuzioni Linux)

# PROCEDURA
Attivare Hyper-V in Windows (Pro?)
Installare Ventoy su SSD esterno, usando le opzioni NTFS e GPT.
SSD > Creare la cartella \ventoy e copiarci dentro il plugin per leggere i dischi VHD/VHDX (si trova sul sito di Ventoy).
Gestione disco > Creare un VHDX dinamico da almeno 50GB formattato in NTFS, e inizializzarlo.
Rufus > installare Windows to-go nel disco VHDX.
Gestione disco > Smontare il VHDX.
Hyper-V > nuova VM, che monti il file VHDX come disco, e avviarla > completare la procedura di primo avvio Windows, e chiudere la sessione.
Copiare il VHDX nell'SSD Ventoy, insieme ad eventuali altri file ISO.
