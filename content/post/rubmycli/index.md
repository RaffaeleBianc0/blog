---
title: "rubMyCLI"
description: "La mia configurazione completa di Windows Terminal, con una selezione curata di tool CLI"
date: "2026-09-20"
lastmod: "2026-09-20"
categories: 
  - "script"
  - "tecnologia"
image: "images/wt.gif"
draft: false
---

Questo script arriva con qualche anno di ritardo su queste pagine: lo ho messo insieme mentre ero a casa col covid durante la pandemia, lo ho usato decine di volte da allora, ma non mi era ancora venuto in mente che potevo pubblicarlo.  

In quelle giornate di reclusione mi sono intrippato un sacco con PowerShell e il microcosmo di tool CLI (Command Line Interface, quindi strumenti da linea di comando, senza le consuete finestre da cliccare col mouse) che neanche pensavo esistesse... _"chi vuoi che utilizzi ancora l'interfaccia a caratteri in Windows?"_  

E invece...! Sicuramente non c'è la cultura della CLI radicata come nel mondo Linux, ma da quando esiste PowerShell il divario si è ridotto di parecchio, e in generale vale la pena mantenere un po' di confidenza con questo ambiente perché **alcune attività si fanno meglio nella CLI**, soprattutto se fai un mestiere nel campo dell'informatica.

Quindi dopo l'esplorazione iniziale ho dedicato parecchie (troppe) ore a cesellare ogni dettaglio del terminale, font, colori, prompt, alias, moduli, variabili d'ambiente sia in PS che in CMD, issues aperte sui repo GitHub dei tool più apprezzati: una cosa molto molto nerd, dall'utilità reale tendente a zero, ma che intanto vien fuori una roba bella e chissene dell'utilità, giusto?  
Questo il risultato ottenuto (finora):  
{{< youtube o0MqeateVb4 >}}

Contemporaneamente, dato che sono pigro e che l'idea di rifare le cose daccapo mi mette angoscia, costruivo anche il sistema per ripristinare l'intera impalcatura su qualunque PC con un singolo comando.  
Funziona così:  
{{< youtube QY9bmWhip48 >}}

Ecco, esattamente questo fa rubMyCLI: ripristina su qualunque PC la mia configurazione di Windows Terminal con tutti i software che ho selezionato e i miei file di configurazione, in modo da ottenere esattamente l'ambiente CLI con le funzionalità che ho assemblato durante quell'isolamento da covid più qualche ora ulteriore qua e là.  

Trovi tutto (script + file di supporto + descrizione completa di tutte le funzionalità) qui:  
{{< bottone link="https://github.com/RaffaeleBianc0/rubMyCLI" >}} rubMyCLI su GitHub {{< /bottone >}}
