---
title: "directaCsvConverter"
description: "Converte i dati Directa in formati per Yahoo Finance e Ticker"
date: '2026-09-28'
lastmod: '2026-09-29'
categories: 
  - "finanza personale"
  - "script"
  - "tecnologia"
image: "images/cover.jpg"
draft: true
---

Come broker nel 2024 ho scelto [Directa](https://www.directa.it).  
Per tenere traccia dei rendimenti in modo completo, includendo sia le posizioni aperte sia quelle chiuse, ho usato [Yahoo Finance](https://it.finance.yahoo.com); e per un certo periodo anche [Ticker](https://github.com/achannarasappa/ticker) più che altro per amore verso l'interfaccia a caratteri (poi sostituito con la mia creatura [**pfpeek**]({{< ref "pfpeek.md" >}}) naturalmente).  
Trasportare le informazioni da Directa a questi due strumenti è noioso, perché i formati sono tutti diversi: i CSV esportati da Directa sono diversi dal CSV importato da Yahoo Finance, e ovviamente dal file YAML che usa Ticker.  
Per facilitarmi la vita ad ogni nuovo acquisto/vendita di quote, ho creato **directaCsvConverter**, prima come script PowerShell, poi anche come [SPA (Single-page application)](https://it.wikipedia.org/wiki/Single-page_application) così che sia utilizzabile anche da chi è un po' meno smanettone.  

Trovi la webapp pronta da usare qui:  
{{< bottone link="/directacsvconverter" >}} directaCsvConverter {{< /bottone >}}

La repo Github, comprendente anche la versione PowerShell, è invece qui:  
{{< bottone link="https://github.com/RaffaeleBianc0/directacsvconverter" >}} directaCsvConverter su GitHub {{< /bottone >}}
