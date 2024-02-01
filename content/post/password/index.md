---
title: "Password!"
date: "2016-01-30"
categories: 
  - "tecnologia"
tags: 
  - "password"
  - "sicurezza"
---

Già vista la famosa e illuminante vignetta di [xkcd](https://xkcd.com/936/)? Eccola:

![correct horse battery staple](images/correct-horse-battery-staple.png)

Molto probabilmente usi password _[corte](http://passwordresearch.com/stats/statistic374.html)_ e _[sempre uguali](http://passwordresearch.com/stats/statistic258.html)_. Dovresti pensarci! Ti racconto di come ci ho pensato io.

# Per farla breve

Versione condensata di questo articolo:

> Cambia la tua **_PASSWORD_** in qualcosa come _**...2016X...PASSWORD**_, su tutti i servizi online a cui tieni (email Facebook Twitter Linkedin banca eccetera). _**2016**_ è l'anno corrente (da cambiare dopo ogni capodanno), _**X**_ è l'iniziale del servizio dove hai l'account (F per Facebook, T per Twitter, eccetera), e _**PASSWORD**_ è la parte a tua scelta. Con uno schema di questo tipo, avrai password sufficientemente lunghe, diverse su ogni sito, aggiornate ogni anno, facili da inventare e da ricordare.

Se ti interessa il _perché_, continua a leggere!

# Il problema

Ogni volta che guardiamo la mail sul telefono, rispondiamo a un messaggio su WhatsApp, o buttiamo l'occhio alle notifiche su Twitter, stiamo usando una password. Magari è memorizzata nel dispositivo, ma la stiamo usando! E lo facciamo con con una **frequenza** pazzesca, quotidianamente. Oltre alla frequenza, anche la **diffusione** è alta - almeno, parlo per me: il mio vault [LastPass](https://lastpass.com) conta 503 siti web dove ho un account. _Cinquecentotre_. Certo, molti siti non esisteranno più, e il 90% non li uso mai, ma ad ogni modo gli account a cui tengo davvero sono senz'altro qualche decina.

Se uno di questi account "importanti" mi venisse rubato, sarebbe _un bel fastidio_, per usare parole delicate. **Come potrebbe succedere?** Ci sono almeno queste 2 considerazioni da fare:

1. I database degli account di molte importanti realtà del web **sono _già_ stati rubati** in passato. [Google](http://www.lastampa.it/2014/09/10/tecnologia/rubate-cinque-milioni-di-password-gmail-hacker-russi-sotto-accusa-j4er5VFJ7u4qYXrxUqdvPP/pagina.html), [Linkedin](http://www.ilsole24ore.com/art/tecnologie/2012-06-07/linkedin-milioni-mezzo-password-124628.shtml?uuid=AbHfJgoF), [eBay](http://www.ilsole24ore.com/art/notizie/2014-05-21/cyber-attacco-ebay-portale-web-chiede-utenti-cambio-password-152623.shtml?uuid=ABbIR3JB), [Libero](http://www.oversecurity.net/2014/07/08/libero-mail-probabile-attacco-agli-account-email/), [Sony](http://www.darkreading.com/attacks-and-breaches/sony-hacked-again-1-million-passwords-exposed/d/d-id/1098113?), e chissà quanti altri - compreso lo stesso [LastPass](http://www.telegraph.co.uk/technology/internet-security/11677827/Cyber-attack-breaches-password-database-LastPass.html)! - hanno subito un qualche tipo di compromissione/furto di queste informazioni. E quasi sempre si è trattato di furti di _milioni_ di account. Magari anche il tuo è già in mani sbagliate, pronto per essere crackato dopodomani. Quindi è sbagliato "fidarsi" al 100% in generale, anche dei "nomi grossi", o delle tecnologie consolidate (magari vi ricordate di [Heartbleed](https://it.wikipedia.org/wiki/Heartbleed), ad esempio).
2. Forse usiamo **la stessa password che usavamo 10 anni fa un po' dappertutto**, o se va bene ne abbiamo due diverse _\-_ magari una per le poche cose "importanti" (email, banca e poco altro) e l'altra per tutte le altre cose "non importanti". Anche tu fai così? ;-)

Mettendo insieme i punti 1+2, il risultato è immediatamente questo:

> _Se uso la stessa password un po' dappertutto da 10 anni, e durante questi 10 anni mi hanno rubato uno qualunque di quegli account, allora tutti i miei account sono a rischio_.

Suona male, vero?

Poi probabilmente l'attaccante di turno userà uno strumento che, automaticamente, appena cracka con successo un account di (per esempio) Facebook, immediatamente prova la stessa combinazione "login/email + password" su GMail Twitter Linkedin Tumblr Instagram UniCredit BNL Fineco e altre centinaia di siti. E poi, su ciascuno di quelli dove il tentativo di login va a buon fine, sceglie: o si mette da parte l'accesso ottenuto "per usi futuri", oppure cambia immediatamente la password con una a sua scelta, tagliando fuori il legittimo proprietario. **Suona _molto_ male, vero?**

Ora, è chiaro che i miei account non sono granché interessanti da rubare rispetto a quelli di un miliardario o di una star di Hollywood. **Ma non è questo il punto.** Il punto è che questi attacchi vengono quasi sempre eseguiti su milioni di account non necessariamente "selezionati": l'esposizione a questo rischio non è correlata al portafoglio, insomma. **Siamo _tutti_ a rischio**.

# A me è successo

Un bel po' di anni fa mi sono trovato 4 acquisti completati su eBay, per un totale di più di 3000€ da pagare. Acquisti che ovviamente non avevo mai fatto. Ho parlato con altre 2 persone a cui è successo, e che sono dovute passare attraverso una denuncia alla Polizia Postale per risolvere. Io sono stato più fortunato perché ho risolto semplicemente seguendo le procedure di segnalazione con eBay, però ho dovuto comunque dedicare un paio d'ore a capire quali fossero queste procedure e ad applicarle. **Avevo una password debole**, fatta solo di 9 lettere minuscole (che ovviamente ho cambiato in quell'occasione, anche perché eBay al tempo possedeva PayPal e... non si sa mai). Ma quello che era peggio è che **la stessa password l'avevo usata per _decine_ di account** su altri siti. Quindi, oltre alle 2 ore perse per eBay, ho dovuto dedicare qualche altra ora per fare il "giro" dei miei account a cambiare la password. Davvero un modo poco interessante di passare il tempo!

# Le password _dovrebbero_ essere...

Il problema n°1 delle password, "lato utente", è che devono essere **[facili da ricordare](http://passwordresearch.com/stats/statistic262.html)**. E questa caratteristica fa a botte con tutte le caratteristiche che invece sono raccomandabili, e che sono più o meno queste:

- E' bene usare una password **differente per ogni account**.
    - Questo per evitare che, una volta rubatoci un account, ce ne vengano rubati altri N solo perché la login/email e la password che abbiamo usato sono le stesse.
    - [Questo studio](http://www.webroot.com/us/en/company/press-room/releases/protect-your-computer-from-hackers) ci racconta ad esempio che circa metà degli utenti Facebook nel 2010 usava la stessa password dell'account Facebook su altri siti.
- E' bene **cambiare periodicamente** ogni password.
    - Questo darà meno tempo utile ad un eventuale attacco "a posteriori" su database di account rubati magari qualche mese prima.
    - [Questa statistica](http://www.statista.com/statistics/305455/millennials-generation-x-frequency-of-password-changes/) dice che circa il 60% dei giovani americani cambia le proprie password almeno una volta all'anno. Avrei scommesso che la situazione fosse molto peggiore di così!
- E' bene che le password siano **lunghe** (diciamo almeno 12 caratteri).
    - Oggi è possibile noleggiare risorse computazionali online, ottenendo una potenza di calcolo inimmaginabile fino a qualche anno fa, e in crescita continua! Dato che il tempo necessario a crackare una password con metodi brute-force ha andamento esponenziale rispetto alla sua lunghezza, è bene puntare all'uso di pass_phrase_ che contengano molti caratteri. La vignetta di xkcd più sopra suggerisce esattamente questo.
- E' bene che le password includano **caratteri presi da più insiemi** tra questi: lettere minuscole, lettere maiuscole, numeri, simboli.
    - Questo fattore probabilmente oggi è utile soprattutto per far sì che la password rispetti eventuali vincoli che molti siti ancora impongono durante la creazione dell'account, che magari consentono di scegliere una password di soli 4 caratteri, purché ci siano dentro una cifra e un simbolo. Quello che conta _molto_ di più è la cruda _lunghezza_ di una password!
- E' bene che le password non coincidano con **parole da dizionario** (in qualunque lingua).
    - Questo perché una tecnica fruttuosa per indovinare password è il _[dictionary attack](https://it.wikipedia.org/wiki/Attacco_a_dizionario)_, e relative modifiche (aggiungendo prima/dopo delle combinazioni di 1/2/3/4/5 cifre, e/o giocando con maiuscole/minuscole, e/o usando 2/3 parole affiancate, e/o giocando con le sostituzioni _[Leet](https://it.wikipedia.org/wiki/Leet)_ come "p@55w0rdd1ff1c1l3" invece che "passworddifficile", eccetera).
    - Un buon tasso di successo ha anche l'uso di un dizionario composto dalle password più usate, come [questo](http://www.whatsmypass.com/the-top-500-worst-passwords-of-all-time) - suggerisco di darci un'occhiata, per farsi un'idea di come spesso sia sottovalutato il problema!

Insomma creare delle password "sicure" sembra una **gigantesca rottura di scatole**, vero? :-)

# La mia soluzione

Ho pensato a una soluzione semplice, che consente allo stesso tempo

- facilità di **creazione** di una nuova password quando serve
- rispetto di **tutte (!)** le caratteristiche sopra elencate
- facilità di **memorizzazione**

L'idea è quella di cambiare la nostra attuale

> ### _PASSWORD_

con qualcosa simile a

> ### _...2016F...PASSWORD_

... perché:

- **Inizia con un segno di punteggiatura**, invece che con una lettera o cifra (una scelta statisticamente meno probabile rispetto alle [password più usate](http://www.lifehacker.com.au/2015/01/doh-the-25-most-popular-passwords-of-2015/), il che non guasta).
    - [Questo studio](https://www2.trustwave.com/rs/815-RFM-693/images/2015_TrustwaveGlobalSecurityReport.pdf) a pagina 106 dà un'idea sui pattern più utilizzati per costruire una password. Quel capitolo è molto interessante in generale.
- Include la _PASSWORD_ che **già usate e ricordate**, e che può essere anche relativamente semplice, perché il resto dei caratteri che ci aggiungiamo prima la rende abbastanza lunga e complessa in ogni caso.
- Il "." è un simbolo che esiste in **qualunque tastiera** di qualunque dispositivo, ed è sempre **in prima battuta** anche su smartphone/tablet: quindi non obbliga a premere \[Shift\] né a commutare la tastiera alfabetica in quella dei simboli, rendendo la digitazione più rapida.
- Include l'anno corrente: in questo modo, quando arriva il 2017 **è immediato capire che è ora di cambiare la password**.
    - Un cambio di password all'anno non è male, anche se c'è qualche sito che obbliga a cambiamenti più frequenti.
    - [Questo studio](https://www.giac.org/paper/gsec/16274/analysis-password-aging/117428), anche se un po' vecchiotto (è del 2009), conclude che per una password "robusta" il fatto che resti immutata per lungo tempo non aumenta significativamente la sua debolezza rispetto ad un attacco brute-force. Viceversa, una password debole è _molto_ soggetta al problema.
- Dopo l'anno, c'è una lettera maiuscola che è l'iniziale del nome del servizio a cui stiamo associando l'account - "F" per "Facebook" ad esempio. Questo rende la password **automaticamente diversa (quasi) per ogni sito**, senza renderla impossibile da ricordare. Per togliere quel "quasi" e dormire sonni tranquilli, si potrebbe scrivere _per esteso_ il nome del servizio - insomma "FACEBOOK" invece di "F", ottenendo anche una password enormemente più sicura, però un po' scomoda da digitare.
    - Si potrebbe pensare che _un solo carattere_ di differenza non aiuti granché sul fronte della sicurezza, ma va tenuto conto che i database degli account memorizzano (quasi sempre) le password non in chiaro, ma "_hashate_" con qualche algoritmo, e **un singolo carattere diverso fa cambiare _totalmente_ un hash** - per provare questa cosa in 10 secondi si possono calcolare [in questa pagina](https://www.tools4noobs.com/online_tools/hash/) gli hash per le due stringhe "prova1" e "prova2" usando l'algoritmo MD2 proposto di default, ottenendo rispettivamente "c2ab7a75856a61ab8e7feca9276108d8" e "89034ca8d78229201b7e3f92e61a33ae".
- La parte "anno+lettera" è _non alla fine_ della password. Forse incide poco, ma anche il fatto che la differenza tra due password non sia alla fine sembra avere un minimo peso, stando a [questo studio](https://www.lightbluetouchpaper.org/2011/02/09/measuring-password-re-use-empirically/). A parità di sforzo, tanto vale annegare questa differenza a metà della password.
- Usa 2 sequenze di punti per "abbracciare" la combinazione anno+lettera, così diventa **più lunga restando facile da digitare e da ricordare** (casomai scegliete di usare 4 o 5 "." se la vostra _PASSWORD_ è troppo corta)
- Combina punteggiatura, maiuscole, cifre (e anche minuscole, se la vostra _PASSWORD_ ne prevede): ottimo, tutti e 4 gli insiemi sono utilizzati! Quindi nessun sito rifiuterà questa password perché ritenuta "troppo semplice", e **lo schema sarà valido ovunque**, senza costringerci a gestire delle eccezioni.
- E' **facile da ricordare: è sempre lo stesso schema**, una volta pensato è già imparato!
- La cambiamo 1 volta all'anno, e siamo indotti a farlo "automaticamente" mentre la digitiamo, ma soprattutto è **_comoda_ da cambiare**, perché non costringe a inventarsi nulla di esoterico: lo schema è sempre uguale, e il cambiamento di un solo carattere da "2016" a "2017" ha le stesse conseguenze positive sull'hash già scritte più sopra.
- E' **sufficientemente lunga**, perché alla vostra _PASSWORD_ stiamo aggiungendo almeno 11 caratteri, quindi il totale è sicuramente >14 caratteri. Ottimo anche per quei (rari) siti più attenti che chiedono password lunghe almeno 12 caratteri.

# Varianti e aggiunte

**PIN** Se ti piace di più, invece di una _PASSWORD_ puoi usare il _PIN_ del tuo telefono, ottenendo qualcosa come _**...1234...2016F**_ che totalizza comunque 15 caratteri e mantiene tutte le caratteristiche che ho descritto. Meno robusta perché c'è solo una lettera, ma tutto sommato adeguata. Magari usa più punti: in _**.....1234.....2016F**_ ci sono 19 caratteri.

**PASSPHRASE** Se hai già in mente una _PASSPHRASELUNGA_ già di suo, puoi viceversa pensare ad uno schema più compatto del tipo ._PASSPHRASELUNGA2016F_: un solo punto all'inizio, >20 caratteri, c'è l'anno, c'è la lettera sempre diversa alla fine... non male!

**PUNTI** Ancora, puoi scegliere di esagerare con i punti costruendo un'idea semplice, tipo: .........Nove2016F -> 9 punti, poi ancora "9" scritto in lettere, e il solito anno+lettera, per un totale di 18 caratteri, in una password robusta, facile da ricordare e digitare, unica, croccantina, quadrata, pratica, buona.

**2FA** Dove è disponibile, e buona cosa sfruttare la "[2-factor authentication](https://en.wikipedia.org/wiki/Two-factor_authentication)" per proteggere i tuoi account. Ad esempio GMail, Facebook, Linkedin la supportano, e puoi vedere su [questo sito](https://twofactorauth.org/) quali altri servizi la supportano e in che modo. E' un miglioramento alla sicurezza che supera qualunque password complessa, e non ha controindicazioni pratiche. Si tratta di fornire al servizio il proprio n° di cellulare, in modo tale che ogni volta che avviene un tentativo di login da un _nuovo_ dispositivo, il servizio manda via SMS un codice da digitare per poter completare il login. Ricordati di impostare sempre una "scappatoia", nel caso tu perda il telefono! Questo vale soprattuto per l'[Account Google](https://accounts.google.com), se la tua email è su GMail: configura una email di riserva (ad esempio quella di lavoro, o dei familiari), in modo da poter ottenere in qualunque caso l'accesso al tuo account, imposta qualche numero di telefono di backup nel caso venga perso l'accesso al telefono principale, ed eventualmente stampati i "Codici di Backup" (o salvali da qualche parte online, in modo che siano recuperabili _senza_ necessità di usare GMail).

**LASTPASS** Per gestire le mie password in maniera comoda mentre sono al PC uso [LastPass](http://www.LastPass.com), che offre una serie di funzionalità eccellenti tra cui la compilazione automatica, l'eventuale generazione automatica di password sicure, un check del livello di sicurezza delle proprie password, indicazioni sul fatto che la stessa password sia usata su più siti, eccetera eccetera. Preferisco questo strumento, invece che memorizzare le password direttamente nel browser. Forse però sarebbe più sensato abbandonare anche questo strumento e adottare solamente la soluzione mnemonica che propongo in questo articolo, per evitare ulteriori possibilità di furto dei propri dati... ci penserò.

# Link

Ecco qualche link correlato a quanto ho scritto:

- [HowSecureIsMyPassword.net](https://HowSecureIsMyPassword.net/): utile per avere un'idea di massima su quanto sia "buona" una password - magari digitateci qualcosa di _simile_ alla password che avete in mente, invece che proprio _uguale_... non si sa mai, giusto? ;-)
- [GRC "How big is your haystack?"](https://www.grc.com/haystack.htm): circa come sopra, ma più dettagliato, e soprattutto contiene molte considerazioni interessanti sul tema.
- [PasswordResearch.com](http://passwordresearch.com/): soprattutto la pagina delle [Statistics](http://passwordresearch.com/stats/statindex.html#User Password Practices), per farsi un'idea di massima dei comportamenti, e il [blog](http://blog.passwordresearch.com/).

# Conclusioni

Mi è sembrata un'idea semplice da mettere in pratica, ma allo stesso tempo efficace.

Ora si tratta di fare il giro dei primi account importanti che ti vengono in mente, e cambiare dappertutto quella vecchia password... ;-)
