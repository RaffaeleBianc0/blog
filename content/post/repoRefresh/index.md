---
title: "repoRefresh"
description: "Mantiene il tuo repository locale con le versioni più recenti degli installer"
date: "2026-08-19"
lastmod: '2026-08-19'
categories: 
  - "tecnologia"
image: "images/repoRefresh.gif"
draft: false
---

Questo script PowerShell mantiene aggiornato un repository locale di installer di applicazioni Windows.  

Anni fa curavo il **mistomareXP**, una mia "distribuzione" su CD (poi DVD) che installava WinXP, lo configurava secondo i miei gusti, e installava una selezione di software, tutto automaticamente.  
Poi ovviamente i dischi ottici sono spariti dalla circolazione, ma la cartella "mistomare" nei miei computer c'è ancora.  

Per tenerla aggiornata, a tempo perso scaricavo i setup delle varie applicazioni.  

Oggi uso repoRefresh, perché fa tutto lui: controlla ogni applicazione elencata nel file apps.CSV, e se c'è una versione più recente disponibile scarica il setup nella cartella specificata.

Lo trovi qui, con tutti i dettagli:  
{{< bottone link="https://github.com/RaffaeleBianc0/repoRefresh" >}} repoRefresh su GitHub {{< /bottone >}}
