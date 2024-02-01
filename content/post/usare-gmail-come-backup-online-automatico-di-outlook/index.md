---
title: "GMail come backup di Outlook"
date: "2010-01-22"
categories: 
  - "tecnologia"
tags: 
  - "gmail"
---

[![](images/gmail.jpg)](http://www.kevinscrate.com/blog/wp-content/uploads/2009/01/gmail.jpg)

Per gestire le mail di lavoro, uso Outlook. Un po' per abitudine, un po' perché si integra senza sforzo col telefono WinMobile.

Mi piacerebbe poter usare GMail ovviamente, ma il massimo a cui sono arrivato è inviare le mail che al destinatario appaiono con il mittente in questo formato: "Da: MioIndirizzo@GMail per conto di: MioIndirizzo@Lavoro".

Per carità, tutto funziona, se il mio interlocutore fa "Rispondi" la sua email arriva correttamente al MioIndirizzo@Lavoro, ma cmq non è ancora tutto ok per almeno questi 2 motivi:

- se scrivo alla mailing-list aziendale, dato che sto usando il server SMTP di GMail per l'archiviazione automatica della posta che spedisco, il messaggio viene rimbalzato. _E-razzismo._
- se i clienti memorizzano nella propria rubrica il MioIndirizzo@GMail e iniziano a scrivermi lì, io mi ritrovo a dover consultare DUE mailbox invece di una. _Una basta e avanza._

Pazienza: ho rinunciato al mio obiettivo iniziale.

Ho deciso però di tenermi quel MioIndirizzo@GMail come **backup automatico in tempo reale** di tutta la posta che invio e ricevo tramite Outlook. Questo perché mi capita spesso di essere da clienti, e di dover accedere alle mie email senza avere il notebook operativo e/o collegato a internet... poter accedere a tutta la mia posta con la potenza di GMail non è da poco - soprattutto per i 7.5GB di spazio e la ricerca istantanea. (Proprio questi due sono in fondo i miei motivi principali per cui passare a GMail...)

Senza entrare nei dettagli di ogni singolo passaggio, ecco quanto ho fatto:

1. Ho attivato un nuovo account su GMail - proprio quel MioIndirizzo@GMail che dicevo sopra.
2. Nelle impostazioni del MioIndirizzo@GMail, ho collegato il MioIndirizzo@Lavoro, in modo da poter sia inviare che ricevere tutta la posta di lavoro.
3. In Outlook, ho impostato l'account del MioIndirizzo@Lavoro in modo che lasci una copia dei messaggi sul server, rimuovendoli dopo qualche giorno.
4. _Ecco il passaggio chiave:_ sempre in Outlook, seguendo le istruzioni che ho trovato qui [http://www.outlookcode.com/article.aspx?id=72](http://www.outlookcode.com/article.aspx?id=72) (Method #1), ho fatto in modo che nel CCN di qualunque email io spedisca venga messo automaticamente il MioIndirizzoGMail. La cosa interessante è che, nel MioIndirizzoGMail, **la posta che invio da Outlook appare correttamente come "Posta _Inviata_" anche in GMail**, e non come _ricevuta_!

Risultati:

1. Ogni email che ricevo, appare anche nella Posta in Arrivo del MioIndirizzo@GMail.
2. Ogni email che invio, appare anche nella Posta Inviata del MioIndirizzo@GMail.
3. Continuo a usare Outlook esattamente come ho sempre fatto - zero operazioni aggiuntive.
4. Quando mi serve ho tutte le email con tutti gli allegati sempre disponibili online, sul MioIndirizzo@GMail.

Prossimo passo: sbarazzarmi dell'ARCHIVE.PST (2.5GB ad oggi...), facendone l'upload sul MioIndirizzo@GMail e trasformando le cartelle in Etichette. Credo che tramite una combinazione di qualche tool + Mozilla Thunderbird + qualche sua extension + l'accesso IMAP al MioIndirizzo@GMail si possa fare... ma non ho ancora indagato a fondo.
