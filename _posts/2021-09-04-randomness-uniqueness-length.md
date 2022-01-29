---
layout: post
categories: privacy security
share: false
image:
  path: images/2021-09-04-randomness-uniqueness-length.png
  thumbnail: images/2021-09-04-randomness-uniqueness-length.png
  caption: Randomness, uniqueness, length, my personal archive
title: Randomness, uniqueness, length
excerpt: Nel nostro quotidiano inseriamo una marea di password. Se misurassimo il tempo che in una vita passiamo a pensare alla giusta password che dobbiamo inserire o a provare la seconda, terza, quarta parola chiave potrebbe tranquillamente risultare che abbiamo passato ore se non giorni della nostra vita a gestire il problema delle password. Oggi provo […]
---
Nel nostro quotidiano inseriamo una marea di password: se misurassimo il tempo che in una vita passiamo a pensare alla giusta password che dobbiamo inserire o a provare la seconda, terza, quarta parola chiave potrebbe tranquillamente risultare che abbiamo passato ore se non giorni della nostra vita a _gestire il problema delle password_. Oggi provo a dare qualche suggerimento per, eventualmente, gestirlo al meglio e liberarvi di questa preoccupazione tipica del nostro tempo.

Partiamo dall’inizio: una password, oltre ad essere evidentemente una parola chiave per accedere ad una risorsa dove non tutti hanno diritto ad accedere, è frutto dell’equilibrio, che scegliamo noi, fra _capacità di resistere ad un attacco e capacità di ricordarcela_. Una password da sola non ha valore, fa parte di un insieme di “coordinate” necessarie per accedere alla risorsa di cui sopra: nel nostro quotidiano, quelle minime, sono username e sito web/app per accedere alla risorsa e, talvolta, un ulteriore codice (il 2FA che vediamo dopo).

Per cui, per fare un esempio, se vogliamo accedere all’informazione “il mio saldo sul conto corrente” ci occorre considerare:

* Sito della banca
* Username
* Password
* 2FA (che per le banche è obbligatorio)

Replicando questo per tutti i servizi che ogni giorno usiamo si capisce bene che la nostra testa non ci può star dietro se non, secondo un errato senso comune, “ottimizzando” un pochino: cerchiamo di usare sempre lo stesso username – ma può essere difficile: omonimie, non ci piace più la user di tre anni fa, a volte la user è la mail, a volte abbiamo più mail, etc. – oppure proviamo ad usare la stessa password o, peggio, entrambe le cose.

È in questo momento che possono nascere i problemi, innanzitutto perché per quanto forte (cioè fatta con tutto l’insieme della tastiera: simboli, minuscole, maiuscole, numeri, geroglifici, etc.) se la stessa chiave apre più porte allora è solo questione di tempo prima che qualcuno, una volta scoperta, la vada a provare su tutte le altre porte possibili (social network in primis) guadagnando così l’accesso a tantissime nostre informazioni con cui di solito si confezionano i migliori attacchi possibili. Di solito quando un sito si fa sottrarre le nostre credenziali, perché incapace di custodirle, se ne accorge tardi quando queste sono già state diffuse spesso assieme ad altre informazioni personali: chi ne entra in possesso proverà – a costo zero e con buona probabilità di successo – ad accedere ad altri siti/servizi. Utilizzare la stessa password quindi può crearci danni di grande entità sia economica (richieste di riscatti per informazioni, prelievi dal conto, utilizzo delle carte di credito, etc.) che psicologica (senso di violazione, perdita del senso di sicurezza personale propria o altrui, etc.).

Anche usare una password debole può essere pericoloso. Un esempio di password debole è il nome del proprio gatto, un’informazione che spesso si può anche dedurre dai social network, così come il nome dei figli, la squadra del cuore, etc. Le password deboli sono, appunto, deboli, perché facilmente deducibili da chi ci sta attorno: con i social network e in generale con tutto quanto riversiamo online purtroppo occorre considerare nel “chi ci sta attorno” chiunque possa guardare i nostri profili e cioè, spesso, una moltitudine incontrollata di persone. Parole di senso comune sono poi spesso usate di default in quegli attacchi, molto semplici, in cui si provano in continuazione tutte le possibili parole di un determinato vocabolario (dictionary attack).

Ci sono poi i 2FA – two factor authentication – cioè quei codici temporanei che _in qualche modo_ vengono generati da app sul nostro telefono o inviati a noi tramite sms. I 2FA sono molto importanti perché sono un _livello di sicurezza_, non una password, in più e andrebbero abilitati ovunque sia possibile farlo. I 2FA aggiungono al processo di autenticazione un livello: se con la username indichiamo “chi siamo” e con la password comunichiamo qualcosa che solo noi dovremmo poter sapere, con il 2FA dimostriamo che, in più, abbiamo anche una cosa che solo noi dovremmo poter avere. Uso il condizionale perché sia le password che i telefoni/numeri di telefono possono essere sottratti dai legittimi possessori, anzi è estremamente facile in Italia almeno finché non si rinforzeranno le procedure di portabilità seguite dagli operatori. Ne avevo già parlato [qui](https://www.fabiolucidi.it/2020/12/29/acchiappafantasmi-forse-ne-abbiamo-bisogno/), si chiama _sim swap attack_.

Ad ogni modo, long story short, le password migliori sono quelle che cadono nell’intersezione di questo diagramma che ho disegnato solo per voi (l’idea esisteva già su internet, ma su questa mia bellissima opera sto pensando di fare il mio primo NFT…).

<figure class="align-center" style="width: 580px">
  <a href="#"><img src="{{ 'images/2021-09-04-randomness-uniqueness-length.png' | absolute_url }}" alt=""></a>
  <figcaption>Un mio diagramma: Randomness, Uniqueness, LenghtLook.</figcaption>
</figure>

Randomness significa _pesantemente casuali_, cioè generate casualmente da un qualsiasi generator ad elevata entropia (includendo sempre tutti i caratteri possibili della tastiera).
_Uniqueness_ significa che le password devono essere davvero uniche: per ogni servizio che usiamo serve una password diversa.
_Length_ significa _lunghe il massimo possibile consentito_ dal sito così da rendere quanto meno più costoso un _brute-force attack_ (provare tutte le combinazioni possibili di caratteri).

Ma come si coniugano password lunghe, tutte diverse e soprattutto generate a caso con la “capacità di ricordarcela” di cui parlavamo all’inizio? Qui ci arriva in soccorso un particolare software: il password manager.

Un password manager è un software che ci aiuta in tutti i processi relativi alle password: *generarle, conservarle, proporcele quando sono necessarie* (cioè nelle relative schermate di login), e in diversi casi *mantenerle sicure*. In realtà si occupa anche di tutte quelle _coordinate_ che dicevamo prima e i migliori sul mercato gestiscono anche i 2FA in modo da inserirli direttamente senza SMS/App specifica.
Ce ne sono diversi “in commercio” ma da anni ormai alcuni con funzioni basilari sono già incorporati nel OS (è il caso di KeyRing delle principali distribuzioni Linux e macOS) o nei browser (LockWise di Firefox e sicuramente altri che non conosco).
Essendo però un tipo di software particolarmente importante e sensibile (contiene tutte le nostre credenziali!!!) va valutato con attenzione soprattutto dal profilo di sicurezza e privacy: organizzare e ricordare per noi le password è una cosa, conservarle in maniera sicura un’altra. Proprio per questo il team di ProtonMail ne ha [considerati e valutati alcuni sotto molti profili](https://protonmail.com/blog/open-source-password-managers/) e, conoscendo l’attenzione che prestano ai temi di privacy e sicurezza, mi sento di dire che se il vostro non è in nell’elenco sarebbe meglio cambiarlo. Di sicuro se non è open source non lo troverete: se non è open source il codice non è verificabile da terzi e di conseguenza non può essere considerato sicuro.
Viceversa, se ne state cercando uno il loro post è un ottimo punto di partenza.

Con un password manager quindi risolvete i vostri problemi di password su qualsiasi dispositivo (si installa su pc, tablet e telefoni e anche come estensione del browser per integrarsi al meglio): al contrario della canzone ora abbiamo risolto mille problemi – tutte le nostre password sono più sicure – e ce ne resta uno, proteggere la password del password manager 🙂

Questa password o master password o master key – ogni servizio la chiama a modo suo – di fatto proteggerà tutte le altre quindi è molto importante, come dicevamo prima:

* Che ce la ricordiamo (purtroppo potremmo essere il peggior nemico di noi stessi)
* Che sia forte (scegliamo noi il livello di “randomness” e lunghezza)
* Che sia unica
* Che sia accompagnata da un 2FA [^1]

[^1] Il 2FA più diffuso è sicuramente il codice sul telefono, ma come visto può esserci sottratto a nostra insaputa mettendoci fuori gioco per un certo tempo, per questo il supporto più affidabile, laddove supportate, sono le security keys (Solo, Yubico, etc.) non solo per proteggere password manager ma anche per specifici account sensibili: pensate a Twitter per un giornalista d’inchiesta, per un politico esposto, per un soggetto che con una dichiarazione può influenzare il mercato, un account di trading, etc.

In questo modo potremo, estremizzando, non conoscere neanche le nostre password dei vari servizi o siti che usiamo: ci basterà sapere solo quella del password manager, quindi non avendo altri “oneri mnemonici” possiamo anche pensare ad una master password più forte delle nostre solite e, come detto, accompagnarla con un 2FA.

Infine un’ultima cosa: la sicurezza non è un processo one-shot che si fa e poi si può dimenticare, è una procedura periodica come l’igiene dentale, gonfiare le gomme della bici, la revisione della macchina e simili. Tutti i password manager semi-seri aiutano anche a **manutenere le nostre password** con alcune funzionalità come quelle di verifica delle password duplicate (cioè se abbiamo una stessa su più account), delle password deboli e, soprattutto, delle password esposte. In quest’ultimo caso confrontano automaticamente con basi dati pubbliche come [questa](https://haveibeenpwned.com/) se le nostre credenziali sono finite online in chiaro a seguito di un attacco. Come sempre nel campo della sicurezza tutte queste cose sembrano grandissime minchiate o cose da super specialisti e invasati, e se tutto va bene possiamo anche continuare a chiamarle così, purtroppo però è così solo fino a quanto non se ne diventa vittime.

Può sembrare strano ma questo è il primo post che scrivo integralmente da tablet - disegno incluso. Tanti anni fa non pensavo sarebbe mai stato possibile e siccome sono scettico che sia venuto bene al primo colpo chiedo scusa in anticipo per refusi da correttore automatico, formattazioni strane o problemi di layout in generale…soprattutto agli affezionati lettori che ricevono i miei post via email e non beneficiano delle correzioni successive!
{: .notice--info}
