---
layout: post
categories: writings
title: "Come sopravvivere all'inverno (e alle altre stagioni)"
date: 2022-08-11
share: false
image:
  path: /images/2022-08-11-Come-sopravvivere-all-inverno.jpg
  thumbnail: /images/2022-08-11-Come-sopravvivere-all-inverno.jpg
  caption: <a href="https://unsplash.com/photos/A-p_6tFvGF8">Unnamed, a photo by Rythik</a>
excerpt: "Se in questa estate caldissima volete trovare un posto molto fresco prendete il grafico del prezzo di _Bitcoin_: siamo in un periodo che già in passato era stato denominato _crypto winter_, un periodo di prezzi bassissimi dopo le vette di ottobre..."
---
Se in questa estate caldissima volete trovare un posto molto fresco prendete il grafico del prezzo di _Bitcoin_: siamo in un periodo che già in passato era stato denominato _crypto winter_, un periodo di prezzi bassissimi dopo le vette di ottobre.
<figure class="align-center">
  <a href="#"><img src="{{ 'images/2022-08-11-Come-sopravvivere-all-inverno-chart.png' | absolute_url }}" alt=""></a>
  <figcaption>Il sereno andamento del prezzo di Bitcoin</figcaption>
</figure>
Questi periodi sono un toccasana per gli _hodlers_, cioè quelle persone che hanno come strategia la detenzione per lunghi, lunghissimi periodi o addirittura all'infinito. Questi periodi fanno pulizia sul mercato costringendo chi ha seguito strategie di breve termine a uscire dal mercato, registrando magari pesanti perdite, e fanno anche pulizia nella _industry_ facendo crollare i business plan di società del settore prive di valore intrinseco e mal gestite e, più in generale, di tutto ciò che è pesantemente o maldestramente collegato al valore di Bitcoin.

Ogni volta che attraversiamo questi periodi leggo cose assurde. Se da un lato gli _hack_ di [Terra/Luna](https://decrypt.co/100402/how-terra-ust-luna-imploded-crypto-crash) e [Solana (wallet)](https://medium.com/web3-magazine/solana-wallet-hack-explained-f91f3fc1cbeb) mi hanno affascinato (col dovuto rispetto per chi ci ha perso), dall'altro mi domando come sia possibile che molte persone continuino a commettere gli stessi errori che già si sono visti in passato. Sembra lungo, ma non lo è, ci sono solo molti esempi e link :)

Allora ho pensato di fare un piccolo decalogo (o _eptalogo_?) commentato, sperando che possa salvare qualcuno in futuro.
1. **Se non è Bitcoin è una shitcoin** \
Magari antipatico ma vero: tutto ciò che è venuto dopo Bitcoin non ha innovato di un _h_ questo mondo, ha fatto al massimo promesse interessanti da esplorare tecnicamente ma che personalmente ritengo non sicure e non affidabili per poterci puntare sopra più di un tappo di bottiglia. **Stare sempre alla larga dalle _shitcoins_ per semplificarsi la vita**: una cosa in meno da rendere sicura significa vita più semplice.
2. **Not your keys, not your bitcoins** \
Se non sei l'unica persona esistente ad avere accesso (aka conoscere) la tua _private key_ non puoi considerare i tuoi bitcoin  al sicuro, perché chiunque altro la conosca può *legittimamente* movimentarli. Si applica anche alle _altcoins_ o _shitcoins_ semplicemente perché queste non nascono dal nulla ma derivano concettualmente da Bitcoin. **Se compri o peggio tieni i tuoi bitcoin su un exchange sappi che tecnicamente non sono i tuoi bitcoins, sono i loro**. Se un exchange non permette o rende eccessivamente onerosi i prelievi in bitcoin lascialo il prima possibile.
3. **Proteggi la tua private key** \
Ovvia quanto diretta conseguenza del punto precedente: ma come si fa?
    + La _private key_ non deve **mai risiedere su un dispositivo che può accedere ad internet**, perché significa che vi si può anche accedere _da_ internet (concetto di _hot wallet_, cfr. hack di Solana), quindi non va tenuta sul telefono (anche per altri motivi), tablet o pc (ma meglio quest'ultimo del telefono: si può usare [Electrum](https://electrum.org/) con alcune accortezze, ma è comunque sub-ottimale).
    + Il posto migliore è un _cold storage wallet_: [Ledger](https://shop.ledger.com/pages/ledger-nano-s-plus), [Coldcard](https://coldcard.com/), [Jade](https://blockstream.com/jade/), [BitBox02](https://shiftcrypto.ch/bitbox02/bitcoin-only/), etc. coprono tutte le esigenze per facilità d'uso, opzioni, configurabilità, etc.
    + Averne un **backup**: su carta (che però brucia), nella propria testa (che però perde colpi), su [superfici di acciaio](https://bitcoinseedbackup.com/) o addirittura una [capsula d'acciaio](https://cryptosteel.com/)
    + Verificare periodicamente che il proprio backup sia **integro e non alterato**.
4. **Proteggi la tua identità** \
Non sto suggerendo di scomparire nel nulla :) ma solo di **rendere il più difficile possibile l'associazione fra l'identità reale e gli indirizzi bitcoin** usati. \
Un soggetto (o peggio un'istituzione) in grado di associare un nostro indirizzo alla nostra persona può costringerci con diversi mezzi e livelli di forza a disporre dei nostri bitcoin come preferisce: un malintenzionato con minacce fisiche, un'autorità giudiziaria con un sequestro, e così via. \
Alcune **buone prassi** in ordine di facilità:
    + Evitare il riutilizzo dello stesso indirizzo per ricevere da soggetti diversi.
    + Fare a meno di soggetti che richiedono contemporaneamente le due informazioni come per esempio gli exchange (Coinbase, Binance, Crypto.com, etc.) e chiunque richieda un KYC: puoi agevolmente fare a meno degli exchange usando servizi come [HodlHodl](https://hodlhodl.com/) o [Bisq](https://bisq.network/), [RoboSats](https://learn.robosats.com/) o altri.
    + Far [girare un proprio _full node_ BTC](https://raspibolt.org/), per non dover usare servizi di terzi per consultare i saldi degli indirizzi,  interfacciandosi ad esso preferibilmente via TOR.
5. **Non parlare mai dei tuoi bitcoin** \
Blocca chiunque ti contatti per parlarne o chi offre servizi quali custodia o supporto di vario genere a meno che non hai la massima certezza e fiducia nel tuo interlocutore. Ovviamente questo deve escludere la possibilità di parlare di Bitcoin in generale come tema, ma è in ogni caso buona norma **non parlare mai con nessuno dei propri bitcoin** (quanti sono, dove sono, da quanto tempo, come li hai acquistati o venduti, etc.). Le conversazioni sui social meritano ancora maggiore attenzione, così come i contatti via email.
6. **Don't trust, verify** \
Una massima (e un [post]({% post_url 2021-01-17-not-your-keys-not-your-bitcoin %}) da tenere sempre a mente e molto legata al punto 4.3: la verifica diretta è sempre da preferire a quelle indirette. Se per esempio qualcuno ti dice che ti ha mandato un certo importo in bitcoin, **non fidarti** del link che ti manda per dimostrartelo, ma **verifica indipendentemente** (col tuo nodo o con uno di terzi se non ne hai uno tuo) se quella transazione che dice esiste davvero e il numero di conferme che ha.
7. **Se non conosci approfondisci, se conosci approfondisci lo stesso** \
Come direbbe qualcuno _let's see how deep the rabbit hole goes_: Bitcoin è un mondo sconfinato e la profondità con cui puoi affrontare un tema è anch'essa smisurata, c'è sempre da imparare e più ne sai più facile sarà evitare _scam_ e rischi in generale.
