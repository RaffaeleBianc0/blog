---
title: "directaCsvConverter"
description: "Converte i dati Directa nei formati per Yahoo Finance e Ticker"
date: '2026-10-04'
lastmod: '2026-10-04'
categories: 
  - "finanza personale"
  - "script"
  - "tecnologia"
image: "images/cover.jpg"
draft: true
---

Per i miei investimenti nel 2024 ho scelto [Directa](https://www.directa.it).  

Per tenere traccia dei rendimenti in modo completo, includendo sia le posizioni aperte sia quelle chiuse, sto usando [Yahoo Finance](https://it.finance.yahoo.com); e per un certo periodo ho usato anche [Ticker](https://github.com/achannarasappa/ticker) più che altro per amore verso l'interfaccia a caratteri, poi sostituito con la mia creatura [**pfpeek**]({{< ref "pfpeek.md" >}}) naturalmente.  

Trasportare le informazioni da Directa a questi due strumenti è noioso, perché i formati sono tutti diversi, cioè i CSV esportati da Directa sono diversi dal CSV importato da Yahoo Finance, e ovviamente dal file YAML che usa Ticker.  

Per facilitarmi la vita, ho creato **directaCsvConverter**, prima come script PowerShell, poi anche come [single-page application](https://it.wikipedia.org/wiki/Single-page_application) così che sia utilizzabile anche da chi è un po' meno smanettone.  

La webapp pronta da usare è qui:  
{{< bottone link="/directacsvconverter" >}} directaCsvConverter {{< /bottone >}}

La repo Github, comprendente anche la versione PowerShell, è invece qui:  
{{< bottone link="https://github.com/RaffaeleBianc0/directacsvconverter" >}} directaCsvConverter su GitHub {{< /bottone >}}
