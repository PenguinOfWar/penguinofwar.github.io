---
layout: post
title: "Data leaks and good password strategies"
description: "This is an archived post from 2019/01/18 covering the top level subject of data leaks and some recommendations for how to stay safe. This was converted from a presentation I gave to the wider marketing platform within Sony Professional Europe that served as an entry-level knowledge session on the subject."
thumb_image: "posts/apps.jpg"
tags: [apps, ethics, social, data, leaks, privacy, passwords]
---

## Note: I have no monetary interest in any of the recommended apps, sites, and services below. Many of them I pay for and use myself.

There has been a substantial leak of credentials (email address and password combinations) on the internet this week (2019/01/18). A large collection of credential stuffing lists (combinations of email addresses and passwords used to hijack accounts on other services) was discovered being distributed on a popular hacking forum. The data contained almost 2.7 billion records including 773 million unique email addresses alongside passwords those addresses had used on other breached services.

As one of my old (thankfully retired) passwords and my email address was one of the leaks, I thought it would be a good time to share not just some information on good password management practices, but also some tools that I personally use to maintain good password security protocols.

## Use cryptographically strong (read: hard to guess) passwords

There are a few popular methods out there for creating hard to guess passwords.

A good explanation of what has come to be called the “Correct Horse Battery Staple” method was explained in comic form by internet comic publisher Randall Monroe better than I can explain it!

[![](https://imgs.xkcd.com/comics/password_strength.png)](https://xkcd.com/936/)

In essence, a random selection of common words combined together can be easy to remember but hard for machines to break. In this way, we stop thinking about them as passwords and more passphrases. Long passphrases equal more entropy, which results in machines taking much longer to crack them while reducing the risk of somebody else also having the same password!

This method is especially useful for securing your “digital fortress”, for example your Google or Apple account or even your password vault itself.

The most secure password is one you can’t remember

The above method is great for one or two sites, but like me you have probably registered to hundreds or even thousands of sites over the years. How can you possibly remember all of them?

## Answer: don’t!

There are many good options for generating cryptographically strong passwords and storing them in an easy to use way, that never exposes you to the guts of actually generating and storing a good password.

Many modern operating systems such as MacOS, iOS, and Android (chrome specific) ship with built-in support for generating and storing passwords for websites and applications. These passwords are securely shared across your devices and synced to a cloud storage location for backup.

1.                          [iCloud Keychain (MacOS and iOS native functionality, works in browsers and apps)](https://support.apple.com/en-gb/HT204085)

2.                          [Google password manager (Cross platform but Chrome specific and cloud synchronised)](https://support.google.com/chrome/answer/95606?co=GENIE.Platform%3DDesktop&hl=en)

3.                          [Firefox (Cross platform but specific to the Firefox browser)](https://support.mozilla.org/en-US/kb/password-manager-remember-delete-change-and-import)

You’ll notice all of these are platform or browser specific (iCloud Keychain for example is locked to Apple products, which is a shame because in my opinion it’s by far the easiest to use), but thankfully there are other options.

My recommendation for providing secure password vaults in a cross-platform way is [1Password](https://1password.com/).

![](https://i.1password.com/media/getting-started-windows/overview.png)

There are a few options available, a free solution that leaves the concern of backing up and device sharing to you, or a built-in cloud option for a couple of pounds/dollars a month. I personally recommend this option.

## Generating a strong password with 1Password

Highlighted in blue above you’ll see an example of the strong passwords that are automatically generated for you, on a per-site or per-app basis. These passwords are hard to remember, hard to crack, and unique.

Where 1Password really shines is the integrations it has with browsers and operating systems.

1.                          [System wide 1Password integration for Mac](https://support.1password.com/getting-started-mac/)

2.                          [System wide 1Password integration for Windows](https://support.1password.com/getting-started-windows/)

3.                          [Browser extensions for all the common browsers](https://1password.com/downloads/#browsers)

4.                          [iOS app (integrates with keychain for automatic password generation and retrieval)](https://1password.com/downloads/ios/)

5.                          [Android app](https://1password.com/downloads/android/)

Pairing this sort of method with the “Correct Horse Battery Staple” method gives a very strong password security protocol while only requiring you to remember one single password:

1.                          A single, strong, easy to remember password for your password vault

2.                          All other passwords generated and stored in your password vault

[Further reading: The Only Secure Password Is One You Can't Remember](https://www.troyhunt.com/only-secure-password-is-one-you-cant/)

## Don’t re-use passwords across services

This goes without say, but each site you enter a password into is a potential risk for you later. If you re-use a password a lot or use a common password ([Link 1](https://en.wikipedia.org/wiki/List_of_the_most_common_passwords) / [Link 2](https://github.com/DavidWittman/wpxmlrpcbrute/blob/master/wordlists/1000-most-common-passwords.txt)) and one of the sites you are registered for is hacked or your common password shows up in a list, you are [instantly vulnerable](https://securityintelligence.com/its-time-for-users-to-pony-up-and-quit-reusing-passwords/) on all other sites that share that password and email combination.

## Use two-factor authentication where possible

Two-factor authentication is an extra layer of security for your various accounts designed to ensure that you're the only person who can access your account, even if someone knows your password.

In 2019, most sites that matter have some form of two-factor authentication and I strongly suggest you use wherever possible, especially on your email account, banking, or e-commerce sites such as Amazon.

[This link](https://support.apple.com/en-gb/HT204915) outlines simply how Apple achieves two-factor authentication, but the principle is the same almost everywhere.

Most two-factor authentication systems use:

1.                          Text/phone calls with unique codes to trusted phone numbers

2.                          An app such as Google Authenticator or Authy to generate expiring tokens

While there is some discussion about the security of text/phone calls (specifically around the risk of cloned numbers/SIM cards), ultimately it doesn’t strictly matter how you are doing it, just that you should be doing it.

And if someone is trying to access your life by cloning your phone… you’ve probably got bigger concerns anyway.

As a top tip, if you are currently using Google Authenticator for anything (or get prompted to when you’re definitely following my advice and setting up two-factor auth for your accounts) I recommend swapping to Authy. It’s a drop-in replacement that doesn’t require resetting your accounts if you swap or lose your phone/device.

[Authy vs Google Authenticator](https://authy.com/blog/authy-vs-google-authenticator/)

## Be proactive, not reactive

When a breach happens, you cannot count on the mainstream media to report it or even for the company that was breached to tell you about it. Here is where I recommend taking matters into your own hands.

Thankfully, some security conscious and very smart people have set up an excellent website for tracking every single breach, not just the high-profile ones.

### [Have I Been Pwned](https://haveibeenpwned.com/)

The number of accounts Have I Been Pwned tracks is now over 6 billion and growing every day. It has various tools for checking whether your account or specific passwords have been leaked:

1.                          [General account checking](https://haveibeenpwned.com/)

2.                          [Specific password checking](https://haveibeenpwned.com/Passwords)

Take it one step further, and sign up to be notified when your email is found in a new leak by clicking **“Notify me”** in the header and registering your email address. It’s free and completely secure – I have registered and I’ve been notified each time my email has appeared in a leak or password dump.

And for the ultimate in security, integrate Have I Been Pwned with 1Password and get notified on a per password basis if your password is compromised using a feature in 1Password called [Watchtower](https://www.troyhunt.com/were-baking-have-i-been-pwned-into-firefox-and-1password/).

More information about what makes that process secure is found at the above link.

--

Full details on the incident and more information on how to search the breached passwords are provided in the blog post [The 773 Million Record "Collection #1" Data Breach](https://www.troyhunt.com/the-773-million-record-collection-1-data-reach/).

*For more information, please re-read this blog post.*

*&copy; 1974 Scarfolk Council.*

___
&nbsp;

sd
