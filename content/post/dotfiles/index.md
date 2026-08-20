---
title: "Dotfiles"
description: "I miei file di configurazione di alcune app, soprattutto CLI"
date: "2026-08-20"
lastmod: '2026-08-21'
categories: 
  - "tecnologia"
image: "images/dotfiles.jpg"
draft: true
---

# Dotfiles?
Sono file di configurazione di applicativi.  
Si chiamano così perché il concetto nasce nel mondo Unix, dove è convenzione che il nome di questi file inizi con il *punto*, che li rende invisibili nell'uso quotidiano.



# Hard links
Normalmente ogni applicativo salva il proprio file di configurazione dove meglio crede.  
Per avere tutti i dotfiles in un unica cartella e *contemporaneamente* anche nella cartella che il programma si aspetta, è possibile sfruttare gli **hard links**.  

Il comando per creare un hard link in Windows è questo:  
`mklink /H C:\dotfiles\secondo.cfg C:\path_originale\primo.cfg`

Il risultato è che qualunque modifica apportata a secondo.cfg sarà contemporaneamente applicata anche a primo.cfg, e viceversa, perché è in realtà lo *stesso* file puntato da due fullpath differenti - come se casa tua avesse due indirizzi per arrivarci.



# GitHub
I miei dotfiles, con un po' di info in più, sono qui:  
{{< bottone link="https://github.com/RaffaeleBianc0/dotfiles" >}}
dotfiles su GitHub
{{< /bottone >}}
