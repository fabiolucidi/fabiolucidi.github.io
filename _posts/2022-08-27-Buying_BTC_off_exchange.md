---
layout: post
categories: bitcoin privacy
title: "Buying BTC Off-Exchange"
date: 2022-08-27
share: false
image:
  path: /images/2022-08-21-buying-btc-off-exchange.jpg
  thumbnail: /images/2022-08-21-buying-btc-off-exchange.jpg
  caption: <a href="https://unsplash.com/photos/uXWPg9uMwt8">Banknote face, a photo by Freddie Collins</a>
excerpt: "When you'll realize our financial world is going to end soon, you may want to start buying some hard money like Bitcoin. The charmer voices of some exchanges will lure you into the market by joining them, but trust me: **you've to resist**!!! In this post I'll explain why exchanges should be avoided and non-KYC systems, like HodlHodl and Bisq, should be preferred. "
---
In this post I'm going to explain why is important to buy Bitcoin off-exchange in a non-KYC (KYC stands for **K**now **Y**our **C**ustomer) way, showing two main solutions that allow you to buy and sell in a **safe** (i.e. always keeping your funds safe), **private** (i.e. without sharing unnecessary data) and **peer-to-peer** (i.e. without trusting a centralized mechanism) way.
{: .notice}
* TOC
{:toc}

# (Intro) Knowing who you're buying from
When you'll realize our financial world is going to end soon, you may want to start buying some _hard money_, which is a type of money with the desirable property of _holding_ (instead of losing) its value over time, widely accepted and good as a unit of account. Bitcoin is currently the best option you've and, for sure, the best example of _hard money_ we can see, probably in history.

But buying Bitcoin could be tricky nowadays: you probably _enjoyed_ any kind of ad or commercial about how _fast, easy and secure_ is buying _cryptos_ on Coinbase, Crypto.com, Binance, BitMex, etc. which is partly true (it's easy and fast, I won't say it's secure) but for sure it comes with some costs: **the first is the obvious and outrageous _amount of fees_** for the services, **the second is well hidden and it's - as always on the internet of goods and services - your privacy**.

# Exchanges are evil, or at least no good
There's no exchange on heart that will offer you bitcoin without asking for your IDs. And this is a completely legitimate request, because there are some regulations asking them to do so, as well as others asking them to report to one or many authorities how many _choose your currency_ of bitcoin **you** bought/sold last year. Every country has rules for the Exchanges to _protect the customers_ and this is really important since, in the past, Exchanges acted over the boundaries of common-sense and putting at risk - often losing - customers' money. So now they have a little more rules: none of these are about how they should work (i.e. minimum provisions, custody requirements, etc.), but just on what they should do to prevent money laundering or terrorism, a very minimum check. This basically means "_be sure of your clients identity_" and that's all they do. So yes, **if you deal on an exchange is secure for them, but it could be very unsafe for you**. There're of course exceptions, i.e. exchanges that keep their (your) funds safe, fully backed by the asset you bought, allowing you to withdraw your assets at low fees but there's no obligation for them to work in a safe way or to show you how they manage your money. \
Good news is that **there's no law forcing you to use a regulated exchange if you want to buy Bitcoin**, and no exchange means also no KYC procedures (i.e. what the Exchanges do when they ask for you ID and other data) which is _really good_ for your privacy. \
In the end an exchange is just an intermediary between a bunch of people who want to sell an _asset_ for _something else_ and a bunch of others who want to buy that _asset_ selling that _something else_. Now put a currency for _something else_ and Bitcoin for _asset_ and you have a Bitcoin exchange. The exchange acts in the middle constantly buying from and selling to these two set of people ensuring that there's always a certain quantity to sell/buy or, in other terms, that there's always a price in the market. They don't do it for free, of course. On the contrary it is quite expensive and, in the meantime, they also get access to many information about you depending on the KYC level they apply.

**Buying off-exchange means buying from a specific person who wants to sell**: there're mainly two ways to do that, **offline** (physical _real world_ transaction) and **online**. The first if quite simple: meet someone at the bar, give him/her money and receive bitcoin at the same time. The second is more interesting and more coherent with what Bitcoin really is:

> A purely peer-to-peer version of electronic cash would allow **online payments** to be sent directly from one party to another without going through a financial institution. [...]
>
>Satoshi Nakamoto

# Why buying off-exchange is important?
Three main reasons to do that. \
The first obvious reason is: **privacy**. Buying off-exchange keeps your data more private because you just need to share your payment data with the counterpart, which is still something but it's, by far, less than what you share with an exchange which is subject to other laws that request them to share this information set with others.
The second is: **safety**, you hold your money. When you're buying on an exchange you're buying the right to see a number on a screen which is often (there're exceptions!) unlinked with any amount in the balance of the exchange. In this case the exchanges are acting in _fractional-reserve banking_ mode, meaning they're selling more than they have based on the idea that it's unlikely that everyone will ask for their money at the same time (in fact, it's a rare event). It's worth remembering that you own bitcoin only if you own the relevant keys. So, you really buy bitcoin only if that exchange sends you, on the address you provide them, that amount. And to go back to point one: now the exchange knows who you're, your spending in bitcoin, one (or more) of your bitcoin addresses and can track you and your money on the blockchain.
Third reason: **knowledge** is needed, so, unless you already know well how Bitcoin works, you'll learn something new during the process. You could see this as an obstacle, I see it as a benefit: buying bitcoin without knowing what you're doing (i.e. buying on-exchange) doesn't help the community at all and expose you to all the risks connected to a partial understanding of the situation, which is, in the end, losing your money (something the exchanges are used to).

Ok, now that the _theoretical_ and _moral_ part is over we can start with the practical part. There are many solutions to buy and sell bitcoin without sharing your yearly net income with a third party, but I'll just focus on two: HodlHodl and Bisq. Again, there're others, but these two are, in my opinion, the main to be discussed.

# HodlHodl <a name="HodlHodl"></a>
HodlHodl is a non-KYC platform - i.e. a website - that let you buy and sell **only** bitcoin (this is a pro, not a cons) against a payment to be completed in one of the many ways that the seller can choose from. It's not an exchange, so you won't find a _market price_ for BTC, instead you'll find many offers to buy or sell it made by individuals.
HodlHodl requires to create an account because is based on a standard _reputation system_, but the only information needed is you email address and, of course, one strong password. To start buying you need to provide a bitcoin address - where you would like to receive your funds - and a second password, the _payment password_. This one is needed to create, together with the seller and HodlHodl itself, the _multisig escrow_ needed to guarantee the finalization of the transaction.
## The escrow mechanism: easy and secure
Without a **central** exchange we need a different _trust_ level among the participants: with _trust_ I mean _an incentive to stick to the buy/sell contract_. As you can imagine a bitcoin seller, in a world without exchanges and escrows, could simply cash in your payment and run without sending your bitcoin or, more likely, you would never send a payment to someone without the certainty to get your bitcoin. **The _multisig escrow_ mechanism solves this, without the need to even know the counterpart!**
The _multisig escrow_ is simply an escrow created with your password, the seller's and the HodlHodl's password (the three _sigs_). Once the seller creates the offer - detailing also how she/he wants to get paid - and the buyer takes that offer, HodlHodl creates the _multisig escrow_ with its password (signature), the seller's and the buyer's. The seller will fund the escrow (literally send the funds reported in the offer from his/her wallet to the escrow address) and, once there, after one or more confirmations, the buyer will pay via the agreed payment method. The seller will then receive the money and unlock the release of the bitcoin funds to the buyer.
The funds will move from the escrow with 2 out of 3 signatures, so if everything goes smoothly (most frequent case) buyer and seller will agree on the final status and the funds will go to the bitcoin buyer.  
## The escrow mechanism: but, what if...
This system has _no incentive to deviate_, but if for any reason something should go wrong one of the party will just not sign or confirm their own part: for example if the seller doesn't receive the money he/she won't release the bitcoin funds to the buyer and open a dispute, if the buyer won't receive the agreed bitcoin he/she won't close the transaction and open a dispute. In either case one of them will open a dispute where the third signature - by HodlHodl - will determine if the funds should go back to the seller (i.e. the buyer can't prove that she/he payed) of the buyer (i.e. the seller is lying about not having received the bitcoin funds).

As you can see the platform will actively take part to the transaction just in case of disputes, in all the other cases they just collect a small fee from the parties for the escrow service.

## Final considerations
HodlHodl is a super easy platform to buy and sell non-KYC bitcoin, allowing a huge variety of type payments (it includes Tesla cars...). The platform doesn't offer (nor impose) a wallet service, so you will manage (i.e. send and receive) everything through your personal wallet (Electrum, Sparrow, etc.): this is key for your funds safety and for your **privacy** because allows you to change the receive address for every single deal you close. All they have about you is your email address and your BTC addresses. Using an email alias service could help improve this aspect as well.
HodlHodl is a website, so there's the chance to take it down (an authority could be interested in doing that) and the privacy of your data is the same you have on any other HTTPS website. In the end it's a **non-KYC _centralized_ exchange**.

# Bisq
Bisq (once Bitsquare) is a **non-KYC _decentralized_ exchange**: yes, it's decentralized. Bisq is not a web-based platofrm, instead it is a software you can run on your computer. The application is pretty straightforward so I will focus on the mechanism and **architecture**. The first thing to know is that **Bisq doesn't require you to create an account with your email**: to start trading you just need a valid payment method (SEPA, Swift, Wise, etc.) and **a starting minimum amount of bitcoin**, mainly due to the escrow mechanism as we'll see in a moment.

## The escrow
As we already know, without a central authority to guarantee the transactions, we need an escrow mechanism. From a high-level perspective Bisq's escrow mechanism could look similar to HodlHodl's, but it's not.
The system whole is _peer or user based_ and not _account based_ (which is a plus in terms of **privacy**), there's no _reputation system_ either so, from a market perspective, it's almost like being a new user every time you trade. So, to prevent people from being selfish and acting against the rules, part of the seller's deposit is made in advance - at offer insertion - and the same goes for the buyer. **Yes, the buyer has to put something in the escrow too**: in this way they both put in it something they could lose if they won't comply with the offer specifications. And **this is why you need some bitcoin to buy bitcoin on Bisq**: it's a small, initial, amount but it's still something you need.
This _escrow transaction_ is a _2-of-2 multisig timelocked_ transaction. This means that the funds will be unlocked under one or two circumstances:
- if both (seller and buyer) sign the transaction
- if one of them publishes the transaction once the timelock is reached (10 days from the deposit circa).

Note that, in the first case, the transaction will unlock the funds sending them to the buyer, in the second the funds are set to be sent to a different _recipient address_: the Bisq DAO address, we'll see the reason of this choice in a moment talking about the arbitrator.

So if everything goes smoothly - 99.99% of the cases - you'll fall in the first case: you pay the price to the seller, he receives the money and release the funds to your address by signing the transaction you already signed (i.e. you both sign the _2-of-2_ release transaction). You'll then receive the bitcoin amount you bought **and** what you've put in the deposit, **minus** some little _service fee_ and _mining fee_.

## Any issue?
But you could still have a chance of facing issues with your seller: it could be naive to think the opposite. If you've an issue with the other person you can, as a **first measure**, chat (there's one for every trade) and try to solve the issue directly. If this doesn't work out there's a **second level of resolution** which is the _mediation_ process, which is activated by one of the party if something goes wrong **and** once the trade period is over. It's simply a try by one Bisq mediator that asks for details to both parties and propose a way to solve the issue: if both parties agree the trade is closed and everyone is happy, if one or both disagree the can go through a **third level of dispute resolution** which is the _arbitration_. This is activated once the _timelocked transaction_ is broadcasted (the one that sends all the funds to the Bisq DAO) and after an arbitrator is called in. The arbitrator asks for details to the parties and decides who's right, then _personally_ pays the right side of the trade and asks the Bisq DAO to be repaid for that.

## The network
The second, probably the main, feature of Bisq is the network: Bisq runs on a peer-to-peer TOR network (for the Italian speakers I wrote about TOR [here](/privacy/security/cipolle/)). This is a design choice that hits at least two objectives: it's more **privacy oriented**, since not a single data is store on a central server (there aren't) and it's **more resilient**, since the TOR servers are harder to seize by the authorities or hacked by anyone. In the end, you're the one and only holder of **all** your information, at any point in time. Bitcoin included, of course.

## Final considerations
Bisq is probably the only system that offers this level of privacy and safety, it runs on a peer-to-peer TOR network that requires a specific software - probably a minus if you enjoy web-based trading platform (which is centralized by design) - but **doesn't ask anything about you**. It just requires a payment method and a small initial amount of bitcoin to start buying a bigger amount. It's a **non-KYC, (fully) _decentralized_, exchange**.
This could be a barrier but there're different ways to get an initial non-KYC bitcoin amount ([here's a guide](https://bisq.wiki/Getting_your_first_BTC)).
