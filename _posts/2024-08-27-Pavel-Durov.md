---
layout: post
categories: writings
title: "Pavel Durov"
date: 2024-08-27
share: false
image:
  path: /images/2024-08-27-Pavel_Durov.jpg
  thumbnail: /images/2024-08-27-Pavel_Durov.jpg
  caption: <a href="https://unsplash.com/photos/queen-and-woman-kneeling-beside-sleeping-man-painting-Agvr-2DFZDM">Queen and woman kneeling beside sleeping man, a painting from the Birmingham Museums Trust</a>
excerpt: "Pavel Durov was arrested in Paris on Saturday, August 24, 2024. The coverage provided by the Italian press on this news was initially very modest, and much of the information shared regarding the Telegram platform has been inaccurate. With this post, I would like to clarify two points: the first is that..."
---
Pavel Durov was arrested in Paris on Saturday, August 24, 2024. The coverage provided by the Italian press on this news was initially very modest, and much of the information shared regarding the Telegram platform has been inaccurate. With this post, I would like to clarify two points: the first is that **Pavel Durov is a complex and, above all, elusive figure**, not comparable in my opinion to his Western counterparts in the industry; the second concerns **Telegram itself, which should not be considered a secure messaging platform**, contrary to what the newspapers suggest with reasoning that goes something like __if you can use it to sell illegal things, then it must be secure__.

Pavel Durov’s story has been reconstructed in several newspapers, but in a nutshell: he’s good at designing and marketing a product, his brother is a talented computer scientist, and the logical consequence is the creation of products that the market needs. Initially, in 2006, VKontakte was born, the most widespread “old-fashioned” social network in Russia, and then, in 2013, Telegram.

However, there’s a problem: the Russian government. After a back-and-forth with companies and people linked to the Russian government, in 2014, the Durovs abandoned VKontakte (and Russia) to focus on Telegram, whose company is, more wisely, based in Dubai. In this tug-of-war with the Russian authorities, Pavel Durov resisted requests for censorship and for user data disclosure by Russian authorities, adopting the role of a defender of freedom of speech.

However, the development of Telegram, always entrusted to his brother, doesn’t tell the same story. To **guarantee** - and I really want to emphasize the word **guarantee** - technically and technologically the freedoms of opinion, expression, and speech, it is necessary that _transparency_ and _security_ are the default. In the case of Telegram, both are lacking.

Let’s start with _security_. One of the serious inaccuracies I have repeatedly read in major Italian newspapers about Telegram is that the conversations are encrypted: this is false. Telegram conversations _can be encrypted_, but by default, they are not. If you tap _new message_ and choose the person you want to write to, you will not start an encrypted chat but a plain chat that uses Telegram’s proprietary protocol (MTProto). This protocol encrypts the message from the phone to the server, unlike the end-to-end encryption of Signal’s protocol (also used by WhatsApp, Google, and Signal itself). This is a significant problem because, to this day, no one knows what happens on Telegram's servers, which are obviously numerous and globally distributed: hence the problem of _transparency_. If a protocol cannot be fully verified, it is good practice not to consider it secure: we do not know if anyone besides Durov has access to Telegram’s server code. However, we do know that it would be technically possible to obtain it, and many might be interested: three-quarters of Russian citizens use it, it’s the eighth-largest social network in the world, and it has more active users than X.

It’s the coexistence of these two points that makes Telegram both vulnerable (and appealing): one or more authorities with sufficient coercive power could force Pavel Durov to hand over - decrypting them - the personal information of his users (messages, conversations in general, but also files, considering that the ability to send files up to 2GB is one of Telegram’s most appreciated features). In the case of WhatsApp or Signal, it is not technically possible for this to happen, and this is not a minor issue because e2e encryption is currently the best way to ensure the right to privacy in correspondence, _mathematically_ preventing the state (understood as a concept and not as the Italian, French, or any other state) from intruding into the most personal sphere of the citizen.

In Italy, many articles have focused on the fact that Telegram is used for illegal purposes: this is true, but it’s not the security of the platform’s communications that makes it preferred for these uses (in fact, it would be the opposite) but all the other features, primarily the ability to hide your phone number.

But does this kind of anonymity imply a crime?

Personally, I try never to expose my phone number because I know it could end up in the telemarketing grinder (a still unresolved problem in Italy), and this feature of Telegram suits me well: is it an undesirable purpose? If you were a Russian journalist able to warn on your Telegram channel where the next missile strike in Ukraine was headed, would you prefer to do it with your phone number visible or with an alphanumeric username that cannot be traced back to you?

If you can easily buy fake documents or drugs on Telegram, it’s because, unfortunately, it’s **generally easy** to buy them, and the same goes for weapons and all sorts of illegal activities. It’s not Telegram that enables these transactions and crimes, but it certainly facilitates communication, just as other outdated means did in the past, such as radios, telephones, or newspaper ads. You cannot criminalize a technology designed to protect communication between individuals and sacrifice it for the inability to conduct investigations in another way or to prevent a crime: those who want to commit a crime will find another way to communicate how to do it.

It would be like thinking of banning paper and pen because a mafia boss could use them to write _pizzini_.
