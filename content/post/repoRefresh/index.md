---
title: "repoRefresh"
description: "Mantiene il tuo repository locale di installer aggiornandoli alle versioni più recenti"
date: "2026-07-01"
lastmod: '2026-08-19'
categories: 
  - "tecnologia"
image: "images/repoRefresh.gif"
draft: false
---

Ho fatto questo script PowerShell per mantenere aggiornato il mio repository locale di installer di applicazioni Windows.  

Anni fa curavo il **mistomareXP**, una mia "distribuzione" su CD (poi DVD) che installava WinXP, lo configurava secondo i miei gusti, e installava una selezione di software, tutto automaticamente.  
Poi ovviamente i dischi ottici sono spariti dalla circolazione, ma la cartella "mistomare" nei miei computer c'è ancora, farcita di setup che uso di tanto in tanto su nuovi PC o nuove VM.  

Per tenere aggiornata questa cartella, scaricavo i setup delle varie applicazioni quando mi andava: un lavoro noioso e meccanico, quindi candidato ideale per una automazione.  

Oggi uso repoRefresh, e fa tutto lui: controlla ogni applicazione elencata nel file apps.CSV, e se c'è una versione più recente disponibile scarica il setup nella cartella specificata.

Lo trovi qui, con tutti i dettagli:  
{{< bottone link="https://github.com/RaffaeleBianc0/repoRefresh" >}} repoRefresh su GitHub {{< /bottone >}}
