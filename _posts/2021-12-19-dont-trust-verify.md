---
layout: post
categories: bitcoin raspberrypi security
share: false
image:
  path: /images/2021-12-19-dont-trust-verify.jpg
  thumbnail: images/2021-12-19-dont-trust-verify.jpg
  caption: <a href="https://unsplash.com/photos/f3Yk7gW6chM">Green and black computer, a photo by Stefan Cosma</a>
title: Don't trust, verify
excerpt: Qualche settimana fa ho deciso che avrei dato vita ad un piccolo progetto domestico che, prima o poi, viene voglia di intraprendere a chiunque decide di dedicarsi a Bitcoin. Ho pensato che fra una cosa e l’altra ormai è da cinque anni che mi interesso e parlo dell’argomento e quindi è giunto il momento di […]
---
Qualche settimana fa ho deciso che avrei dato vita ad un piccolo progetto domestico che, prima o poi, viene voglia di intraprendere a chiunque decide di dedicarsi a Bitcoin. Ho pensato che fra una cosa e l’altra ormai è da cinque anni che mi interesso e parlo dell’argomento e quindi è giunto il momento di sostenere il network con un full-node sempre attivo. Incomprensibile? Vado con ordine…

_Far girare un nodo_ significa avere un software sempre attivo connesso alla rete (spiego poi cosa fa): avevo già fatto quest’esperimento nel 2016, ma poco dopo avevo abbandonato l’operazione perché era troppo “pesante” per il mio computer – da cui tra l’altro scrivo ora – non come potenza richiesta ma come uptime e alla fine era più un disagio per me che una reale utilità per il network.

Non era e non è neanche la prima volta che contribuisco con dell’hardware, dell’energia elettrica e della banda della rete a progetti collettivi: in passato ho contribuito al progetto SETI@home contribuendo all’analisi dei segnali raccolti da alcuni telescopi, ma in questo caso lo scopo era assieme molto preciso e poco tangibile.

Mantenere un nodo bitcoin è qualcosa che invece può avere un’utilità rilevante nella diffusione di un sistema libero dall’intermediazione, che non conosce il termine _debito_, non censurabile, ma soprattutto interessante da studiare. In più un nodo in più sulla rete, se ben configurato, dovrebbe aumentare la _qualità del servizio_ complessiva e di sicuro aumenta il grado di _privacy_ di chi lo utilizza.

# Di cosa si tratta?

_Far girare un nodo bitcoin_ significa far girare sul proprio pc il software [bitcoin core](https://github.com/bitcoin/bitcoin) che raccoglie e distribuisce le transazioni e i blocchi di transazioni (validandoli) a tutti gli utenti o servizi che ne fanno richiesta: significa in poche parole essere parte attiva del network rendendolo più affidabile e capillare. Per Bitcoin, un protocollo nato per lo scambio di valore, le _informazioni fondamentali_ da diffondere sono ovviamente le transazioni (“Tizio ha dato 10 a Caio”) e il raggiungimento del consenso sui blocchi (“Siamo tutti d’accordo che Tizio ha da 10 a Caio”): se tutti siamo allineati su queste cose il network è in salute e il protocollo può funzionare al meglio. L’importanza del lavoro svolto dai nodi della rete è proprio diffondere velocemente queste informazioni.

# Perché farlo e cosa serve?

Un nodo bitcoin è tanto più utile al network quanto più è disponibile, ossia attivo (“online”), e veloce da raggiungere. Avere un computer acceso tutto il tempo con questo scopo non è affatto una cosa scontata, in termini soprattutto di consumo energetico, ed è quello che mi ha fatto desistere quando avevo provato nel 2016…di fatto però i requisiti sono sempre gli stessi: un PC con 500Gb liberi e una connessione è tutto ciò che serve.

Negli anni sono cambiate diverse cose – il mio pc non è tra queste 🙂 – e di recente si sono incrociati il desiderio di una persona importante di regalarmi un [Raspberry Pi](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/), il Natale in avvicinamento e una nuova ondata di interesse personale al tema, questa volta un po’ più orientato alla parte tecnica. Morale della favola, a inizio dicembre ho rotto gli indugi e sono arrivate a casa (in netto anticipo sul Natale!!!) queste cose essenziali per iniziare il mio progetto:

* Raspberry Pi 4 model B - [Link](https://thepihut.com/collections/raspberry-pi/products/raspberry-pi-4-model-b)
* Alimentatore ufficiale - [Link](https://thepihut.com/collections/raspberry-pi-power-supplies/products/raspberry-pi-psu-eu)
* Case per Raspberry Pi 4 - [Link](https://thepihut.com/products/flirc-raspberry-pi-4-case)
* Hard disk 1TB USB 3.0 - [Link](https://www.amazon.it/gp/product/B07994QL95/ref=ppx_yo_dt_b_asin_title_o09_s00?ie=UTF8&psc=1)
* microSDHC - [Link](https://www.amazon.it/gp/product/B084CJLNM4/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&psc=1)
* Cavo ethernet - [Link](https://www.amazon.it/gp/product/B07QJ9TVLY/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1)

La cosa che ho capito leggendo in giro è che l’unica cosa fondamentale – a parte il Raspberry in sé – è l’alimentatore ufficiale perché pare che con altri modelli possano esserci salti di tensione: a parte questo gli altri elementi si possono scegliere secondo proprio gusto, budget, preferenza tenendo però conto che la blockchain adesso occupa circa 400Gb e può solo a salire, quindi un disco da 500gb non sarebbe la mossa più lungimirante. Al contempo un disco SSD dà un vantaggio notevole in termini di trasmissione dati a fronte di un costo maggiore.

Ammetto che quando avevo progettato di fare questa cosa avevo pensato di scrivere anche una guida passo passo ma la documentazione online è così abbondante da renderlo inutile: personalmente ho preferito seguire [questa](https://raspibolt.org/) (RaspiBolt), ma inizialmente ero indeciso se seguire [questa](https://howchoo.com/bitcoin/run-bitcoin-full-node-raspberry-pi) o [questa](https://github.com/rootzoll/raspiblitz). Ho optato per la RaspiBolt per una questione di semplicità, chiarezza e attenzione sui temi di _privacy_ (leggi TOR), ma tutte hanno come presupposto il far girare _bitcoin-core_ per cui erano, per il mio scopo, equivalenti: tutte richiedono di scaricare e indicizzare la blockchain di Bitcoin (_not pruned_), operazione che richiede un po’ di tempo (vedi tabella sotto).

In sostanza, senza appunto scendere nella spiegazione passo-passo, il poco hardware necessario e la semplicità delle guide disponibili dimostrano quanto sia alla portata di chiunque creare il proprio nodo Bitcoin, una scelta che permette di sostenere la rete e non dipendere da terzi – siti o servizi disponibili online – per trasmettere le proprie transazioni, verificare i propri indirizzi o qualunque altra operazione che richieda di interrogare la _chain of blocks_ di Bitcoin…permette di applicare a pieno il principio del _don’t trust, verify_, non aver bisogno di fidarsi di nessuno ma di verificare in maniera indipendente le informazioni che ci servono.

| Ril.  | Date and Time (CET) | Progress %  |
| 1 | 2021-12-11 16:00  | 0%  |
| 2 |	2021-12-12 10:28  | 45.46%  |
| 3 |	2021-12-12 17:00  | 57.96%  |
| 4 |	2021-12-13 00:06  | 67.22%  |
| 5 |	2021-12-13 08:42  | 76.26%  |
| 6 |	2021-12-13 12:22  | 80.45%  |
| 7 |	2021-12-13 19:16  | 86.59%  |
| 8 |	2021-12-13 23:44  | 90.01%  |
| 9 |	2021-12-14 09:01  | 94.79%  |
| 10  | 2021-12-14 12:21  | 96.18%  |
| 11  | 2021-12-14 21:23  | 99.94%  |
| 12  | 2021-12-14 21:29  | 100%  |

_Rilevazioni avanzamento download Bitcoin blockchain_
