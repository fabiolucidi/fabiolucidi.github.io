---
layout: post
categories: security bitcoin
share: false
image:
  path: images/2020-12-28-ledger-data-breach.jpg
  thumbnail: images/2020-12-28-ledger-data-breach.jpg
  caption: <a href="https://unsplash.com/photos/riEYPSKxoTw">Star Wars Stormtrooper under Keyboard Key, a photo by James Pond</a>
title: Ledger Data Breach
excerpt: Di recente il mondo di Bitcoin e delle criptovalute è stato travolto da un furto di dati di primo piano. Anche in questo caso – ancor più che in quelli che giornali e siti di informazione chiamano spesso “furti di bitcoin” – non è stata scalfita nè minata la sicurezza del protocollo Bitcoin. La vicenda […]
---
Di recente il mondo di Bitcoin e delle criptovalute è stato travolto da un furto di dati di primo piano. Anche in questo caso – ancor più che in quelli che giornali e siti di informazione chiamano spesso “furti di bitcoin” – non è stata scalfita nè minata la sicurezza del protocollo Bitcoin.

La vicenda in estrema sintesi: **a [Ledger](http://www.ledger.com/), un produttore di dispositivi per la conservazione a livelli di sicurezza militari/paranoici delle chiavi private, è stato rubato un database con le informazioni dei clienti a cui ha spedito i dispositivi acquistati**.

L’episodio può sembrare paradossale, oltre che grave, e di sicuro è imbarazzante per il produttore – costruisci e vendi dispositivi che rappresentano lo stato dell’arte in materia di sicurezza e ti fai soffiare l’elenco dei clienti? – ma ha anche dei risvolti molto critici che vorrei affrontare per mostrare le conseguenze di una perdita di dati e dei rischi per i clienti.

La chiara conseguenza del data breach o meglio del data dump – ossia la pubblicazione dei dati trafugati durante il breach – è che chiunque ne abbia interesse può andare a vedere **l’elenco delle persone che ad una certa data hanno acquistato un prodotto Ledger**. Questi prodotti – gli hardware Wallet di Ledger – sono rivolti a persone che si muovono nel mondo di bitcoin e delle criptovalute, di conseguenza è molto probabile che ne siano anche possessori: **il prodotto di Ledger è rivolto proprio alla conservazione in maniera estremamente sicura di questi asset, una necessità tipica soprattutto di chi ne possiede in quantità**. È quindi evidente che questo database possa fare gola a molti visto il target di persone coinvolto.

Per materializzare al meglio l’idea dei dati messi a disposizione vi riporto un record di esempio, asteriscato per ragioni di privacy, del database trafugato (sul web si può facilmente trovare l’elenco in chiaro completo):

 `********@verizon.net | Matthew ******* | 15** Cedar**** Ln | Frederick MD 21702 | United States | 301********`

Le informazioni sono disponibili per più di **272 mila clienti** – circa 5500 sono in Italia – e sono estremamente attendibili e, di conseguenza, di incredibile valore: **nome, cognome, email, indirizzo e cellulare**. Con “_estremamente attendibili_” s’intende che le informazioni sono – o sono state in un certo istante – veritiere: tipicamente non si inseriscono informazioni false o approssimative quando ci si fa spedire qualcosa a casa. Per chi sa cosa farsene rappresentano una grande opportunità per commettere atti criminali di vario tipo, tanto nel mondo virtuale quanto in quello reale.

Vediamo che **conseguenze ci sono per i vostri Bitcoin** e quali considerazioni possiamo trarre da questa vicenda sulla **raccolta, l’utilizzo e la conservazione di dati sensibili**.

# Su un Ledger Wallet i tuoi bitcoin sono stra-stra-stra-al sicuro, ma…

## 1. Ora qualcuno sa che potresti averli

Tra i dati trafugati un’informazione molto importante è l’indirizzo email usato per acquistare il Ledger Wallet: all’acquisto l’indirizzo email è necessario solamente per ricevere la fattura/ricevuta, gli update sull’avanzamento dell’ordine ed eventualmente la newsletter. **L’indirizzo email è l’informazione più importante per compiere un crimine informatico perchè identifica la vittima ed è la prima leva utilizzabile da un _attaccante_**: se mi spaccio per la società Ledger e ti scrivo alla mail che hai utilizzato per acquistare il Wallet che produco sono più credibile di quanto potrei essere scrivendo ad un indirizzo a casaccio trovato online.
**Il possesso di informazioni specifiche della vittima (_target_) aumenta la qualità e quindi l’efficacia di attacchi**, spesso fortunatamente banali, quali phishing o social engineering. Inoltre l’indirizzo rappresenta un’informazione – la più semplice se vogliamo – della coppia user/password utilizzata per l’accesso a qualsivoglia servizio online: è chiaro quindi che una password debole o peggio sempre uguale indebolisce la sicurezza di qualsiasi altro nostro account (altri data breach hanno esposto le password di molti di noi e combinando le informazioni il rischio aumenta ulteriormente). In sintesi, **la diffusione di un indirizzo email non è mai una buona notizia perchè permettere ad un _attaccante_ di prenderci di mira e di provare a prendere di mira l’email stessa per trafugare a cascata altre informazioni o accessi**.

La 2FA può cambiare nome a seconda del sito su cui la attiviamo, i più diffusi sono: _Two-Factor Authentication_ (2FA appunto), _Two-step verification_, _strong authentication_ o altre locuzioni simili
{: .notice--warning}

In termini di Bitcoin – e protezione degli stessi – l’indirizzo email è un dato di per sè irrilevante ma che occorre comunque proteggere in quanto nostra identità digitale e per farlo **è sufficiente un cambio password e soprattutto l’abilitazione dell’autenticazione a due fattori** (se il gestore della casella email non offre cambiamo indirizzo e gestore), preferibilmente via App (v. più sotto il punto 3). Qualora l’indirizzo email pubblicato sia utilizzato anche per accedere a siti dove si acquistano/vendono Bitcoin è bene accedere a questi siti, cambiare password ed eventualmente anche indirizzo email specie se teniamo lì quantità significative di asset (una pratica che va evitata come la peste…in più perchè farlo se abbiamo un ledger wallet?).

**Se il vostro indirizzo è incluso nell’elenco dei dati sottratti a Ledger e pubblicati è praticamente scontato che riceverete mail di phishing o ransomware di qualche tipo e in qualsiasi lingua: occhi aperti e categorizzate come spam queste email senza perdere tempo a rispondere o ad aprire link di nessun genere (siano essi pagine, documenti condivisi o altro)**.

## 2. Ora qualcuno sa chi sei e dove abiti

In virtù di quanto detto prima – ovvero che le info contenute nel database sono relative a persone potenzialmente interessate ad investire denaro – e del fatto che fra le informazioni rubate vi siano anche indirizzi fisici non è impensabile che a [qualcuno venga l’idea di minacciare fisicamente le persone presenti nell’elenco o entrargli in casa per provare a rubare o farsi consegnare denaro o l’elenco delle 24 parole](https://www.reddit.com/r/Bitcoin/comments/ki5fim/victim_of_ledger_data_leak_receives_phone_call/) che danno il controllo/proprietà dei bitcoin. Questo è senza dubbio l’aspetto più sgradevole e inquietante della vicenda, che fa capire **l’importanza di sapere come i siti a cui diamo nostre informazioni le conesrvino, per quanto tempo e dove**.

Nel caso di un aggressione personale lo spettro delle possibilità di difesa è ampio e variabile e si scontra con la sensibilità di ciascuno, ma limitandoci alla difesa dei soli bitcoin – o meglio delle chiavi private necessarie per muoverli e quindi dimostrare di esserne proprietari – possiamo pensare a conservare l’elenco delle 24 parole in un posto diverso dall’indirizzo finito online o di dividere l’elenco in più parti e conservarle in posti diversi (ma così aumentiamo anche il rischio di perderlo). Un’altra possibilità è creare un wallet con un importo piccolo ed eventualmente consegnare quello in caso fossimo vittima di una simile situazione.

Va detto che, fino ad oggi, sono state poche le segnalazioni di minacce del genere…più spesso nome, cognome e indirizzo vengono utilizzati per mettere la vittima in una condizione psicologica di debolezza per estorcere più facilmente e velocemente denaro. Si torna in questo caso alla fattispecie del ransomware via e-mail (o delle minacce) e di una maggior qualità e quindi pericolosità dei tentativi di phishing. Anche un qualsiasi attacco di social engineering risulterà più semplice e forte avendo a disposizione queste informazioni.

## 3. Ora qualcuno conosce il tuo numero di telefono

Il numero di telefono può sembrare un’informazione marginale ma in realtà è un altro canale di comunicazione utilizzabile da un potenziale _attaccante_, un’altra informazione utile a rafforzare tentativi di attacchi di per se banali (phishing, etc.) nonché **sempre più spesso lo strumento di verifica di accesso ad altri account dove trovare altre informazioni di valore** (account di exchange con asset, account con backup di dati su cui basare ransomware, etc.).

L’importanza del numero di telefono sta nel fatto che la maggior parte dei servizi online lo utilizzano come strumento di verifica di un accesso (la già citata 2FA) inviandoci l’SMS con un numero di diverse cifre da inserire. Ovviamente conoscere il numero di telefono di una persona non permette di ricevere i suoi SMS ma c’è un attacco specifico per farlo: il cd _SIM Swap attack_. Capirlo è molto semplice perchè ne esiste una versione non criminale molto nota: la portabilità telefonica e il ripristino del numero quando smarriamo il telefono e chiediamo il “duplicato” della SIM.

La SIM – _subscriber identity module_ – è l’identificativo della nostra identità, un pezzo di plastica con un chip che l’operatore telefonico sa di aver dato, per esempio, a Fabio Lucidi. Il numero telefonico invece è un’informazione di contatto che l’operatore associa in un secondo momento a quella specifica scheda SIM (da qui per esempio la necessità di aspettare qualche ora/giorno per la portabilità). Da quel momento l’operatore telefonico sa che il tale numero telefonico è da collegare (per chiamate, messaggi, etc.) a quella specifica SIM.

Il **SIM Swap Attack sfrutta la debolezza di questa procedura per associare ad una SIM nella disponibilità dell’_attaccante_ il numero di telefono della vittima (_target_). Questo attacco richiede un certo lavorio, ma nessuna competenza informatica**: occorre solo raccogliere quante più informazioni sul target (cose che spesso si trovano sui social), contattare l’operatore telefonico fingendosi il target e chiedere di procedere con la portabilità oppure ancora corrompere qualcuno che lavori per l’operatore.

Ci si può difendere? Dall’attacco in sè ci devono difendere gli operatori, noi possiamo fare la nostra parte eliminando informazioni sensibili dai social network (dove abitiamo, dove siamo nati, il compleanno, etc.) ma per renderlo eventualmente innocuo **la tecnica migliore è utilizzare come secondo fattore di autenticazione (2FA) le app come Google Authenticator o FreeOTP ed evitare gli SMS**. Il primo campanello di allarme per capire che siamo vittima di quest’attacco è la disattivazione della nostra SIM: il telefono non prenderà più perchè la SIM non sarà più riconosciuta dall’operatore telefonico.

# Su Internet i nostri dati non sono mai al sicuro, quindi…

## A) Se gestisci un’attività online minimizza i dati che raccogli e il tempo per cui li conservi
Tieni sempre presente che la sicurezza è un costo che cresce con il valore e la quantità delle informazioni che custodisci: **se non custodisci nulla non spendi e non rischi nulla**. Per questo è importante limitare al massimo le informazioni che chiedi ai clienti e, in ogni caso, **eliminarle il prima possibile una volta esaurita la necessità di utilizzarle**.

_Esempio: se chiedi l’indirizzo per spedire un prodotto a casa di un cliente eliminalo a consegna effettuata o scaduto il termine di reso._

Se devi (o vuoi) conservare informazioni sensibili devi essere in grado di farlo sempre in maniera sicura (non conservarle in chiaro) e monitorarne periodicamente l’integrità.

## B) Se comunichi spesso i tuoi dati online minimizzane la quantità (solo le info strettamente necessarie!) e usa 2FA e password casuali

Valuta sempre quale tipo di informazione è davvero necessario comunicare, a chi le comunichi (in che Paese risiede, a quali normative è soggetto, etc.) e per cosa autorizzi ad utilizzarle. **Ma soprattutto la prima: le informazioni che non diamo non possono essere rubate e usate contro di noi**.

_Esempio: è davvero necessario comunicare il numero di cellulare a chi mi deve spedire una maglietta dal Portogallo? Mi chiamerà mai questo produttore? Davvero potrebbe servire al corriere che già mi porta centocinquanta pacchi di Amazon al giorno?_

So che è difficile e rognoso ma la pratica più importante per la tutela dei nostri trecentomila account è **l’utilizzo di password sempre diverse e della Two-Factor Authentication quanto meno per gli account più importanti** (Google, Amazon, Twitter, Apple, Samsung, etc.). Per siti di minore rilevanza – ad esempio perchè li usiamo una volta nella vita o ogni sei mesi – **possiamo utilizzare password generate casualmente e conservate da sistemi terzi** come Mozilla Firefox Lockwise, Apple iCloud Keychain (ce ne sono anche altri ma non consiglio ciò che non ho provato) che offrono anche la sincronizzazione fra i nostri dispositivi e verificano per noi se le credenziali conservate sono state diffuse online in data dump analoghi a quello di Ledger, cosa che si può fare anche in autonomia grazie a servizi come https://haveibeenpwned.com.
Infine qualcosa a cui raramente si pensa: **cancellarsi dai servizi che non usiamo più**. È buona norma periodicamente verificare quali servizi non usiamo più e valutare di cancellare l’account.

_Esempio: Ha senso tenere ancora quel vecchio account MySpace? E Flickr? Tumblr? Uso ancora facebook? L’account di MediaWorld che ho usato solo nel 2017 che senso ha? Al massimo se mi serve posso rifarne un altro…)_

Se siete arrivati fino a questo punto vuol dire che avete mostrato un certo interesse per il tema e questa è per me la maggior soddisfazinoe…nella lettura **potrebbe esservi sorta una domanda**: “_ci sei anche tu nell’elenco delle 272 mila persone clienti di Ledger?_”
La risposta è **assolutamente sì** perché, per passione, diversi anni fa avevo iniziato ad approfondire l’argomento Bitcoin – con dei colleghi sotto la guida di Ferdinando Ametrano – e il tipo di sicurezza che i dispositivi Ledger offrono…e visto che di Bitcoin non ho più neanche una frazione vi invito a farmi le vostre laute donazioni a quest’indirizzo: bc1q39e399m4j5r8th533rty4nk7y4rnduevgw8ms8
{: .notice--success}

<figure class="align-center">
  <a href="#"><img src="{{ 'images/2020-12-28-ledger-data-breach-bitcoin.png' | absolute_url }}" alt=""></a>
  <figcaption>bc1q39e399m4j5r8th533rty4nk7y4rnduevgw8ms8</figcaption>
</figure>
