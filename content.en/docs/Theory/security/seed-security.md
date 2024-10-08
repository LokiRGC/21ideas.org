---
title: "Ultimate guide to storing your bitcoin seed phrase backups"
h1: "Ultimate guide to storing your bitcoin seed phrase backups"
cover: /img/secure-seed/vault.png
description: ""
url: seed-security
date: 2022-01-19
bookToc: true
bookFlatSection: false
weight: 3
---

{{< hint btc >}}
This article by Stephen Hall was published in [Unchained blog](https://unchained.com/blog/how-to-store-bitcoin-seed-phrase-backups/).

[Contribute](/contribute/).
{{< /hint >}}

In bitcoin, it’s always important to secure your seeds, but how exactly do you do that? In previous articles, we’ve discussed [what seed phrases are and how they work](/en/seed), and some of the [most common methods for recording them on various mediums](https://unchained.com/blog/seed-phrase-backup-methods-recording-paper-metal/). In this article, we cover how and where to store your seed phrase backups in different bitcoin custody contexts.

# Singlesig vs. passphrase vs. multisig vs. SSSS

When storing your physical seed phrase backups, the first thing you need to determine is which custody model(s) you’re using. These require different considerations because each has security and privacy trade-offs that will affect your storage approach.

For example, singlesig (without a passphrase) involves 12 or 24 words that provide total access to your bitcoin, so in most cases, those words shouldn’t be accessible to anyone but you. Multisig, on the other hand, requires access to multiple keys to be able to spend funds, meaning a key could be lost or stolen without putting your bitcoin at risk — allowing you much more flexibility in how and where you store your seed phrases.

If you aren’t sure which bitcoin self-custody model you should use, there are four primary options to consider:

- Singlesig
- Singlesig + passphrase
- Multisig
- Shamir’s Secret Sharing Scheme

## Singlesig

Singlesig is the most common bitcoin self-custody method — it’s the one with which you’re most likely already familiar. With singlesig, you have one seed generated by one hardware or software wallet and one seed phrase backup; in this case, properly securing your seed phrase is everything! If your seed phrase is compromised, your bitcoin is compromised, because anyone can simply import your wallet and private keys using those words and move your funds.

## Singlesig + passphrase

Singlesig with a passphrase is a step up from singlesig; it’s a middle ground between only using a 12- or 24-word seed phrase and using more redundant models like multisig. In singlesig + passphrase, you add a 13th or 25th word to your seed phrase, which generates a wholly separate and unique wallet. With a passphrase, you avoid the risky practice of using just a seed phrase, but it still allows for single points of failure — if your passphrase is lost, so is your bitcoin.

One important note: It’s easy to conflate **singlesig + passphrase** with **singlesig + wallet PIN** — these are very different things! While a wallet PIN restricts access to your keys, it can be lost or forgotten as long as you still have your 12- or 24-word seed phrase backup, because all a PIN does is protect against access to that specific wallet. A passphrase, however, is required for constructing your wallet itself!

It’s worth noting that you can also combine passphrases with multisig and Shamir’s Secret Sharing Scheme, but in those cases, a passphrase commonly adds unnecessary complexity.

## Multisig

Multisig is a bitcoin custody model where you construct a wallet using multiple keys in an m-of-n scheme. You can create a 2-of-3 wallet, for example, based on **three** keys where **two** are required to sign a transaction. The beauty of this model is that it eliminates single points of failure. Not only could critical items (seed phrase backups and hardware wallets) be compromised without loss of funds, an attacker would also need access to your wallet configuration info to be able to do anything with those keys.

Collaborative custody, the multisig model we use here at Unchained, allows you the benefits of multisig while also getting access to a whole suite of financial services, real human support, access to signing transactions remotely if needed, and much more. A model like this one lets you preserve your sovereignty while also getting the benefits of a trusted partner.

## Shamir’s Secret Sharing Scheme

Another method for protecting your bitcoin is Shamir’s Secret Sharing Scheme (SSSS). The most popular standard for using SSSS in bitcoin is SatoshiLabs’ [SLIP-0039](https://github.com/satoshilabs/slips/blob/master/slip-0039.md), which allows you to split a singlesig seed phrase into a collection of other mnemonic phrases. These can be combined in a scheme very similar to multisig — you can set up a 2-of-3, 3-of-5, or any other scheme that requires a certain number of the parts to be recompiled to construct the original seed phrase. Like multisig, storing your SSSS seed words (which use a different dictionary of words from [BIP39](https://unchained.com/blog/what-is-a-bitcoin-seed-phrase/), by the way) will allow you much more flexibility since any one (or in some cases, multiple) of them being lost or stolen won’t compromise your funds.

# Bitcoin seed phrase storage locations: which to choose?

Just like there are [infinite ways to record your seed phrases physically](https://unchained.com/blog/seed-phrase-backup-methods-recording-paper-metal/), there are infinite places you could store your seed phrases. Some are great, some…not so much.

## Places _not_ to store your seed phrase backups

Many places are poor candidates for storing your seed phrase backups:

- Out in the open
- A drawer/cupboard/shelf
- In a filing cabinet
- In your bag
- At your workplace

{{% image "/img/secure-seed/not-safe.png" /%}}

All of these locations are especially poor choices for singlesig. Generally, anywhere with easy access for potential attackers — or even the fatally curious — is a bad idea.

Even in other redundant models where you can afford to make a mistake, the inconvenience of a compromised or stolen seed phrase or hardware wallet just isn’t worth it — especially when you can store them properly in a safe place with marginally more effort.

## The best places to store your seed phrase backups

### Home safe

**Suitable for**: Singlesig, singlesig+passphrase, multisig, SSSS

One of the most popular places to store seed phrases is a simple fireproof safe. If you have a safe place where you keep important documents and valuable items, it can make sense to hold a seed phrase backup there, too. While storing laminated paper backups in such a safe is likely to be fine, [using a metal backup, which is also fire- and water-proof](https://unchained.com/blog/seed-phrase-backup-methods-recording-paper-metal/) would be even better.

A home safe is one of the best places to store your seed phrase if you’re using singlesig, because you should never trust your seed phrases in the hands of someone else when that seed phrase itself is a single point of failure. The same goes for singlesig+passphrase.

### A second location on your property

**Suitable for**: Singlesig, singlesig+passphrase, multisig, SSSS

A secondary location on your property is another option for both singlesig+passphrase users and multisig. Note that these two areas should be on your property, but hidden and separate enough so that multiple seed phrases won’t be simultaneously destroyed or compromised in an unexpected event like a burglary or fire. If you need to keep two secrets on one single property, you could keep one in a safe in your office and another in a safe under the floorboards or stored in a separate building such as a barn or shed (provided it’s protected from the elements of course!).

Another option is storing your seed phrases in a safe on a second property you own, like a mountain house, lake house, or beach house. Like every other suggestion here, that has trade-offs — those properties are commonly vacant for long periods of time, possibly affording you fewer opportunities for surveillance and/or ensuring your seed phrases haven’t been compromised.

In the case of singlesig+passphrase, you could keep your 12- or 24-word seed phrase in one location and the passphrase in a second location. Or, if you use multisig, you could store two different seed phrase backups on your property where you can monitor and ensure they’ve not been tampered with or compromised.

{{% image "/img/secure-seed/safe.png" /%}}

### Safe-deposit box

**Suitable for**: Multisig, SSSS

Another option is a metal container at an institution with active physical security: a safe deposit box. This option works for multisig or SSSS, because in those cases, you can leave one seed phrase in the hands of a trusted custodian with confidence that your funds could never be compromised with just one unlawful ([or lawful!](https://www.latimes.com/california/story/2021-06-09/fbi-beverly-hills-safe-deposit-boxes-forfeiture-cash-jewelry)) security breach. You can store your seed phrase securely while still retaining control of your funds.

Notably, it’s not a good idea to use a safe deposit box for singlesig or singlesig + passphrase. With singlesig, you’re exposing your funds to unnecessary risk of theft. And even if you add a passphrase, a safe deposit box exposes you to the risk of confiscation. Even if you have your passphrase stored in a separate location, the confiscation of your seed phrase backup will leave you bitcoin-less, even if the confiscating party can’t access your funds.

One thing you may consider is using a safe deposit box within a private vault rather than at a bank, which may allow you more legal protections in the confiscation scenario mentioned above.

If you do use a safe deposit box, you should avoid holding two recovery seed phrases or hardware wallets with the same provider.

### A trusted family member

**Suitable for**: Multisig, SSSS

A trusted family member is another option that only works in a multisig or SSSS context. For example, if your favorite uncle has a gun safe, and you simply need a safe place for one of your three multisig key backups, this can be a great option. You aren’t putting access to your funds at risk when storing only one key with a trusted family member. This won’t work in a seed phrase-only singlesig context because someone else would hold your keys!

If you decide to store secrets with a trusted family member or entity, always ensure they are aware of the responsibility involved in protecting your seed phrases or hardware wallets.

# Every approach is unique

The approach you take to seed phrase storage is highly situational, especially when you start taking into account more advanced self-custody methods such as multisig and SSSS and the wide variety of entity types that hold bitcoin — from personal holders to governments.

{{% image "/img/secure-seed/vault.png" /%}}

A good framework for deciding how to store your seed phrases might be to consider the following for yourself or your organization:

- Are you using the correct custody model (should you use multisig to eliminate single points of failure)?
- What is the current or expected future value of your bitcoin?
- What is the safety status of your country/state/city/neighborhood?
- What unexpected natural disasters could reasonably put your seed phrases at risk?
- Don’t overcomplicate it. Unnecessary complexity is a security threat. You can be your own worst enemy.

# Special singlesig considerations

## Use metal backups

For most singlesig users, metal backups are essential. If you don’t [make your seed phrase resistant to the elements](https://unchained.com/blog/seed-phrase-backup-methods-recording-paper-metal/), the entire value of the bitcoin secured by keys generated by that seed phrase can be gone if just one statistically unlikely event happens. In bitcoin, there is no one to call. There is no bank or government to bail you out. If your software or hardware wallet and seed phrase backups are lost, stolen, or destroyed, your bitcoin is likely gone forever.

## Only you should have access

Not only should you create a metal backup; you should also store that metal backup in a safe place to which only you have access. The only exception to this rule might be the most trusted individual(s) in your life, e.g., a spouse. “Don’t trust, verify,” the saying goes, and few places is that mantra more important than here. Assume that anyone and everyone is interested in your bitcoin or might be in the future.

## Be careful not to say too much

Of all the bitcoin self-custody models, singlesig is where you need to be careful about verbal operational security. If you say too much and someone finds out where your seed phrase is stored, it quickly becomes easy for you to lose all your bitcoin. If a malicious actor wants your bitcoin and knows where to find it, it’s much easier for them to get to it. And remember: just because someone doesn’t care about your bitcoin now doesn’t mean they won’t care in the _future_!

## Consider another custody model

Finally, consider whether singlesig even makes sense for you. If a significant portion of your net worth is in bitcoin or you expect that it may be in the future, you should [consider a collaborative custody multisig vault](https://unchained.com/blog/how-to-create-a-do-it-yourself-unchained-capital-multisig-vault/). With multisig, you don’t have to worry as much about the individual security of a single seed phrase backup because none of the seeds part of a multisig quorum would jeopardize your funds even if fully compromised by themselves.

# Special singlesig+passphrase considerations

Special considerations for singlesig + passphrase are very similar to that of singlesig because ultimately, a passphrase simply protects your 12 or 24 words from being a single point of failure in the case that _you don’t actually lose access to your seed phrase_. If someone manages to steal or destroy all of your seed backups, a memorized passphrase is going to do you very little good. However, it _will_ protect you if someone makes a copy of your seed phrase or you accidentally expose it digitally.

## Don’t trust third parties; don’t trust your mind

For these reasons, you shouldn’t trust your seed phrases in the hands of anyone else, and you shouldn’t store them anywhere but on your property. It’s also generally a bad idea to trust your brain with your passphrase. In the case of a medical issue or an accident, the last thing you want is also to lose your bitcoin. Don’t make your brain a single point of failure when you can preserve your bitcoin for yourself and your loved ones using multisig.

## Two secure locations on your property is fine

Suppose you’re choosing not to use multisig or SSSS for some reason. In that case, you can benefit from the second layer of protection of a passphrase by storing your seed phrase and your passphrase, both inscribed in a metal backup, in separate secure locations on your property. At least, in this case, you can afford to lose your physical passphrase backup (assuming you also have it memorized) without losing your bitcoin.

# Special multisig considerations

If you’ve only used singlesig or passphrases, you’ll find multisig to be the perfect route to a good night’s sleep once you understand how it works. If you create your own 2-of-3 multisig scheme, you can afford to have one key or seed phrase backup entirely compromised or stolen without losing control of your funds. With proper maintenance, this makes your bitcoin self-custody very robust. An attacker would have to understand how bitcoin multisig works, get access to two of your three keys, access your wallet configuration information, _and_ sweep your funds before you realize what’s happening and sweep them yourself.

## More flexibility, but security is still important

Even with the flexibility that multisig affords, you should still take seed phrase storage security seriously and avoid co-locating any hardware wallets or seed phrases. Even if your hardware wallet and seed phrase backups are protecting the same seed, keeping them separated can afford you maximum opportunities to recover your funds before an attacker gets them.

Other than this, your options are wide open: all of the above places we mentioned as good storage locations are acceptable for storing your seed phrases or hardware wallets. Remember, though: there are trade-offs with every option you choose!

## Make your seed phrases more durable

When protecting your seed phrase backups, we recommend laminating any paper backups to make them waterproof at a minimum. We also recommend using metal backups wherever possible to make your seed phrases both fire- and water-resistant. Choose a fireproof safe if you’re storing them in your home, whether using [paper or metal backups](https://unchained.com/blog/seed-phrase-backup-methods-recording-paper-metal/).

# Consider collaborative custody

There are many different approaches to bitcoin multisig. Still, here at Unchained we believe [partnering with a third party to hold the third key in a 2-of-3 quorum](https://unchained.com/vaults/) offers the best set of trade-offs for most people. This approach allows you to remain fully sovereign while also maximizing the convenience of access to funds, and lets you take advantage of financial services to treat bitcoin like generational wealth.

{{< youtube yGgO5RCH0a4 />}}

For 2-of-3 multisig with a custody partner like Unchained holding the third key, you have four important items to protect: two hardware wallets and two recovery seed phrases.

At Unchained, our official recommendation is that you store your four items (two hardware wallets and two seed phrases), geographically separated, in some combination of:

- A primary home safe
- A secondary home safe
- Safe deposit box – Bank A
- Safe deposit box – Bank B
- Safe or safe deposit box (held by trusted family members or trusted entities)

You can [read more about our official seed phrase storage recommendations in our operational security guide](https://unchained.com/blog/wp-content/uploads/2022/01/Unchained-Operational-Security-Guide.pdf).

# Special SSSS considerations

Shamir’s Secret Sharing Scheme has very similar considerations to multisig when it comes to seed phrase storage. You should never store your SSSS shards together in one place; depending on the m-of-n scheme you established when generating your shards, you could be defeating the purpose of using SSSS entirely if you’re not careful about storage locations.

## Avoid unnecessary complexity

In bitcoin security, unnecessary complexity is a security threat. Shamir’s Secret Sharing Scheme isn’t technically any more complex than multisig, but it can become an issue if you don’t know how to properly use the software solutions for generating and combining shards. Even in scenarios where it has made sense historically, such as large organizations distributing key control across multiple people, multisig is still a better approach for most bitcoin holders, especially with user-friendly applications like Unchained vaults.
