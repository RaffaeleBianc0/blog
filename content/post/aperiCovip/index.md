---
title: "aperiCovip"
description: "Confronta i fondi pensione italiani in base ai dati ufficiali COVIP"
date: '2026-08-18'
lastmod: '2026-08-19'
categories: 
  - "finanza personale"
  - "tecnologia"
image: "images/aperiCovip.gif"
draft: false
---

Per scegliere un fondo pensione, specie un FPA, i parametri essenziali sono 2:
- i costi (ISC = Indicatore Sintetico dei Costi, la cosa più importante in assoluto)
- i rendimenti passati (anche se ovviamente non sono garanzia di quelli futuri)

Questi parametri sono pubblicati periodicamente sul sito della COVIP.

Quindi dovresti:
- trovare dove sono questi dati
- scaricarli e aprirli (sono distribuiti in 2 file Excel separati, e pure formattati diversamente)
- mixare le informazioni che leggi su uno dei 2 file con quelle che leggi sull'altro file
- decidere "il migliore" tra i fondi in base al mix dei dati

Per scegliere il mio FPA, a suo tempo ho fatto tutto questo procedimento a mano in Google Sheets.  
Ci ho messo qualche ora.

Per facilitare la vita al prossimo, ho pensato di fare **aperiCovip**, una pagina web che ti guida in 3 semplici passaggi a fare la stessa valutazione, ma con un risultato molto più fruibile e ottenuto in un minuto con pochi click.

Trovi la webapp qui:  
{{< bottone link="/aperiCovip" >}} aperiCovip {{< /bottone >}}

La repo Github è invece qui:  
{{< bottone link="https://github.com/RaffaeleBianc0/aperiCovip" >}} aperiCovip su GitHub {{< /bottone >}}
