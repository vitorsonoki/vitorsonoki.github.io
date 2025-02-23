# The Definitive guide to Password Managers

![digital safe](/static/safe.png)

If you use anything on the Internet today but don't know what a [Password Manager](https://en.wikipedia.org/wiki/Password_manager) is or how to use one, stop right now and read this article until the end. If that's the case, the security of *all* your online accounts is at risk, and it's just a matter of time until an incident happens and compromises one or more of them - a question of *when*, not *if*. 

But it doesn't have to be like this. As pesky as your IT department's or some online platform's password policies may seem to be, dealing with passwords in a secure way doesn't have to be a burden or a hassle. In order to use so many online platforms securely, you should not even need to *think* about all these damn passwords associated with them. In fact, what if you could skip the handling of passwords from your online workflow altogether in a secure way, and just focus on the work what matters instead?

If this sounds like a good idea to you, a Password Manager is *exactly* what you need to start using right now.

This article is a comprehensive guide explaining everything you need to know about Password Managers, and how they make your online life much, much more secure. It begins with an explanation of how they work, the basic usage, and more advanced features are shown towards the end.

## Contents:

 - [How do password managers work?](#how_work)
 - [Why should I use a password manager?](#why)
 - [Types of password managers](#types)
 - [How to use a password manager](#how_use)
 - [What else can your password manager do for you?](#what_else)

<h2 id="how_work">How do password managers work?</h2>

A password manager in a simple sense is a *lockable digital vault*. 

You can store "secrets" like documents, valuables in a vault that you'd like to see later and lock it with a key that only you have. The security lies in having both the access to that vault and to its key at the same time - something that only you as the owner should have.

In the case of the password manager, the vault is the application itself, and the key is the password you use to lock and unlock the vault. And the secrets are your online credentials, usually composed of a username and - you guessed it - password.

Now even though the password manager can store a lot of different types of informations, sometimes even small files, it's optimized for storing *text*, which is exactly what passwords are.

<h2 id="why">Why should I use a password manager?</h2>

The main purpose of a Password Manager is to securely store and manage access credentials. These, in the online world, mean a pair of identifiers: username and password. In order to be considered secure, passwords must have a few qualities to them. For example:

 - Resistant against guessing or "cracking" (the high-speed guessing of millions of passwords per minute done by hackers' through special computers).
 - The longer, the better.
 - Uniquely associated to a single use (no same password for two different accounts).
 - Not recorded anywhere in the clear (no writing down passwords in your agenda, notebook, scrap of paper, text file on your computer, etc)
 - Can be changed quickly and easily in case of issues (compromise, account reset or the good old "I forgot my password" moment)

For example, this would be considered a bad (weak) password:

    B@seball1

And this would be considered a pretty good (strong) password:

    J?zx"ZOKS<&h8P~l$g<[}B]2

The irony is that if you follow all of the best practices above literally, you'll end up with a useless setup: a super secure password... that you cannot by any human means memorize. And remember: you have to have a *different* strong password like this for every single account!

So since memorizing won't work, why don't you store your super strong passwords in a secure location (not in the clear) and then simply *copy and paste them* when you need them? You'd not even have to type them out!

This is where the Password Manager shines: a secure "vault" that you can deposit all your strong access credentials, access them when you need and lock it when not using it.

In other words, a password manager is the **only** way for you to **ensure that all your passwords are strong, unique - and usable**.

There's only one catch: you still need to lock the password manager when you're not using it and the usual of doing that is... with a password! However, if you store all your passwords in that vould *this "master" password is the only password you will ever need to remember*, since every other one will be inside of it. And even if you'd not like to use a password as the lock, there are passwordless alternatives, like using digital key files. 

### What can a password manager protect against?

Let's say that you don't use a password manager, but you do know a thing or two about password strength. You cleverly come up with what you think is a strong password, say:

    Tr0mboner5lyf!

Since you don't want to think up any more unique passwords like that, you just keep using that password everywhere you need to create an account. After all, that *one* password is strong, right? And the websites where you use it will take care of their security too, right?

Turns out one of the websites where you created an account, `jimsfunnyforums.com`, didn't do their security right. Hackers leaked its entire password database in a forum, and your password was included in the clear. Another hacker then picks your username and password from the list, and tries it in a more interesting (and serious) website, say, `gmail.com`.

Since you used the exact username and password from `jimsfunnyforums,com`, the hacker now has complete access to your Gmail account, without having to do any "hacking". And this despite you having used a strong password in first place.

This [attack](https://en.wikipedia.org/wiki/Credential_stuffing), which is [commonplace in the web](https://haveibeenpwned.com/) these days, can be mitigated with a password manager, which ensures that only your `jimsfunnyforums.com` password would be compromised, and not any other. And you can easily change it after it was compromised with another strong password.

### What does a password NOT protect against?

Password Managers are not a panacea, of course, and cannot help you in a few cases. For example:

 - If malware is already present in your computer, and can spy, record or steal information from your password manager without your consent (for example: a [keylogger](https://en.wikipedia.org/wiki/Keystroke_logging)). In other words, if your computer is already infected, a password manager will not protect you against that infection.
 - If the website where you create your account has weak security, a password manager cannot fix *that* insecurity (you might consider *not* creating an account in such websites in first place).
 - Last but not least, a password manager cannot supply you passwords when it's not running. For example, the boot password or disk encryption password of your laptop cannot be retrieved from a password manager because they are required before the password manager can be launched. This applies in other similar environments where the pasting of text is limited or not possible (though you can still type out the password char by char).


<h2 id="types">Choosing a password managers</h2>

There are quite a few choices in password manager software. They can be categorized in a variety of ways, which we'll look in detail now:

<h3 id="cloud">Cloud-based vs Local</h3>

Cloud-based password managers are essentially websites to which you log in through a browser with username and (hah!) password and then retrieve your credentials. Some may require you to log in only via their (more secured) application, but are essentially still just retrieving the data over the internet. 

Others, however, run locally in your computer and their vault is a file stored locally in your device. Those are Local password managers. You run them like you'd run any other program in your computer.

Both of these solutions can be great for you depending on your workflow, and they both accomplish their goals of safeguarding your credentials. There are different pros and cons to either cloud-based or local password managers, however, so you should check them and see what fits better your working model:

<table>
    <tr style="font-weight: bold">
        <td>Type</td>
        <td>Pros</td>
        <td>Cons</td>
    </tr>
    <tr>
        <td>Cloud-based</td>
        <td>
            <ul>
                <li>No extra software required (in case of website-based solution).</li>
                <li>Always have the "latest" credentials across every device you own (synchronized).</li>
                <li>Some solutions can do offline caching, so sometimes you can still access your credentials when offline (provided you've accessed it recently)</li>
            </ul>
        </td>
        <td>
            <ul>
                <li>Requires an internet connection to work properly.</li>
                <li>If the password manager's website gets hacked, all of your credentials are at risk (can't control their security).</li>
                <li>You rely on your Web Browser's security to ensure your credentials are safe (web-based solutions).</li>
                <li>As <a href="https://en.wikipedia.org/wiki/Software_as_a_service">SaaS</a>, it may not be fully Free Software.</li>
            </ul>
        </td>
    </tr>
    <tr>
        <td>Local program</td>
        <td>
            <ul>
                <li>Your credentials never leave your computer. You have full control over them.</li>
                <li>100% functional even when offline.</li>
                <li>Lightweight programs designed with security in mind. Almost all of them are <a href="https://www.gnu.org/philosophy/free-sw.en.html">Free Software</a>.</li>
            </ul>
        </td>
        <td>
            <ul>
                <li>Synchronizing the vault across multiple devices can get tricky about whos's got the latest version.</li>
                <li>There may not be a version for your OS or platform.</li>
                <li>If you lose the password vault file or it gets damaged or corrupted, your credentials are lost forever.</li>
            </ul>
        </td>
    </tr>
</table>

There is the security vs convenience debate involved in this choice, as well as a bit of risk management. You have to analyze which model would work for you, or, even better, try both out and see in practice which one do you prefer.

I personally prefer *Local* password managers in my machines because it gives me full control over where and how my password database is used (including its security). I use the [Git versioning system](https://git-scm.com/) to synchronize and backup the password database across my devices and, this way, avoid overwriting versions and entries as they pile up. Finally, there are versions for all the OSes I use, so I never had a problem of compatibility. But again, this is just my personal opinion, and may not work for you. 

Examples of Cloud-based password managers:

 - BitWarden: <https://bitwarden.com/>
 - Some other Proprietary platforms.

Examples of Local-based password managers:

 - KeePassXC: <https://keepassxc.org/>
 - PasswordSafe: <https://www.pwsafe.org>

<h3 id="browser">Browser-based vs generic</h3>

Did you know that your *browser* itself is a password manager? 

That's right: most if not all modern browsers today offer you some sort of password management feature - they just don't call it by that name! 

For example, when Firefox or Chrome ask you to save a password, guess where they store it? In a password manager-style vault. And they stay protected in there until either you unlock them with a main password or other credentials.

<figure>
    <img src="/static/ff_passwdm.jpg" alt="Password manager in Firefox" />
    <figcaption>
        Firefox comes with a password manager that offer to save your
        passwords as you browse. 
        You can also save additional passwords in it as you wish.
    </figcaption>
</figure>

Even with this great amount of convenience available, however, I would still prefer a *generic* password manager, independent of any browser, like the Local-based ones mentioned before. 

This is because I prefer to separate the duties of the programs I run, much like the classic [Unix Principles](https://en.wikipedia.org/wiki/Unix_Philosophy). Furthermore, in choosing a separate password manager, I'm trusting the security of my passwords to a program *dedicated* to security, rather than one in which security is not the main goal such as a Browser.

However, Browser-based password managers still shine in one special case: when you can't install additional software in the computer you're using. A good example is your work's PC; you probably can't just go and install a password manager in it by yourself. However, you very likely have one or more web browsers available, and can use their password manager feature to store your passwords.

<h3 id="proprietary">Open Source vs Proprietary</h3>

The final distinction I want to make may sound subtle, yet is quite crucial since we're dealing with software in the area of security: **licencing**. 

Most password managers, like KeePassXC and PasswordSafe, are released under Free and Open Source Licenses, and available at no cost. Others are also available free of cost, but are Proprietary in license. While the cost variable is unchanged here, availability of the source code is the big difference between the two. This *is* a big deal here, because having the source code is the *only* way that anybody can inspect the software and attest that it is secure for usage or not.

Free and Open Source software grants you this possibility because source code is freely distributable by definition. That's not the case with proprietary software where the source code is treated as a secret. In the latter, no independent party can audit the software completely, which inevitably results in a higher possibility of bugs and security complications.

For this very reason, I *cannot* recommend any form of proprietary Password Managers, like LastPass or 1Password. You simply cannot trust them completely in their security claims due to their licensing model. I advise you to *always* use an Open Source one.

<h2 id="how_use">How to use a password manager</h2>

Now that the workings and different types of Password Managers are explained, I'm going to show you how to use one, step by step. 

I'm choosing [KeePassXC](https://keepassxc.org/), an open source local-based solution for this. Not only KeePassXC is my favorite password manager, it's also considered something of a Gold Standard of Password Managers and the security community. Naturally, it's what I would recommend you to try as well.

Once you download and install KeePassXC, open it for the first time. The main window will prompt you to either create a new database (i.e. the password vault) or use one you already have. Since it's your first time, you must create one, which you can do right away:

![creating your keepassxc database](/static/keepass01.png)

Add a name and description:

![Describing a keepassxc database](/static/keepass02.png)

You can leave these settings on default. They refer to the encryption mode of the database for compatibility.

![keepassxc database encryption settings](/static/keepass03.png)

Now choose a "master password;" the key that will unlock your vault. This is the only password you'll ever need to remember after you store the others inside it.

![keepassxc database key settings](/static/keepass04.png)

Now choose where you want to save your password database file. **You should remember to back up this file afterwards, as all your passwords will be stored in it.**

![keepassxc database file saving](/static/keepass05.png)

The Password Vault is created. You can now add your first password to the vault. To do this, click the `+` symbol:

![keepassxc new entry](/static/keepass06.png)

Add your username and other metadata to the entry. As for the password you can either type it in if it's pre-existing (not very secure) or let KeePass generate a random, very strong one for you (recommended). To do that, click the dice button. Afterwards, click `Done`.

![keepassxc new entry](/static/keepass07.png)

You now have saved your entry and can access that password by simply copying it from the application and pasting it on the website you need. For that, either right-click your entry and choose from the menu, or use the `Ctrl+B` and `Ctrl+C` keyboard shortcuts.

![keepassxc entry usage](/static/keepass08.png)

<h2 id="what_else">What else can your password manager do for you?</h2>

By now I'm sure I've made your mind about how Password Managers are important for your online security, and also how awesomely easy they are to use. However, it would be unfair to cut the article here without mentioning the extra mile it can go for you in its advanced usage.

In short, besides storing username-password credential pairs, your password manager can also store other important security information (known as *secrets*) related to your accounts, such as:

### Other metadata relating to your credentials

Let's say your account provider adds an extra layer of soft authentication, such as the classic, yet extremely insecure "security questions." If you want to provide a secret (random) value to these without having to memorize them, your Password Manager can store that for you. Just add an *Attribute*, under the "Advanced" tab:

![keepassxc adding metadata](/static/keepass09.png)

You can store as many of these attributes as you need, and they do not need to be strictly secrets either. Examples of things you can store among your credentials in your password vault include: MFA backup codes, random answers to security questions and SSH or PGP keys .

But please, oh please, do not actually use your *actual* information as the answer to your security questions...

### Store MFA secrets, like an "authenticator" token

You know those "authenticator" apps or "security tokens" issued by banks that generate a 6 or 8-digit one-use code for securely logging into their web services? Guess what - KeePassXC can do the same thing.

This is because the way those apps or tokens generate those numbers is no magic; rather, it's a [well-known cryptographic function](https://en.wikipedia.org/wiki/Time-based_one-time_password) that issues a code depending on the current time. The security of that code (which is plainly-readable) lies in the fact that the *secret seed value* used in the generation is kept a secret, and that the code is ephemeral, not lasting more than 60 seconds at max.

What KeePassXC can do is store that seed value alongside your credentials, and generate the one-time code on the spot, which you can then copy and paste into the authentication form. This is an excellent form of backing them up as well, in the event you lose or change authentication options.

### Store PassKeys

Finally, the current next frontier of authentication is [Passkeys](https://passkey.org/). These leverage the strength of public-key cryptography to generate an authentication method that, in the best promises, would allow you to log into somewhere securely without using a password, and maybe even without giving a username at all.

While the standards for PassKeys are still young and evolving, the KeePass team already provide support for it. Much like MFA secrets storage, you can import PassKeys to your password with KeePassXC.

## Conclusion

As we saw in this article, Password Managers are an integral part of digital security and you should integrate one in your online workflow as early as possible. 

Using a password manager to store securely passwords and other credentials is not necessarily difficult, only slightly different than what most people are used to doing. Instead of storing weak passwords in your memory, let the Password Manager generating them securely, and copy and paste them from it. You'll never forget a password this way and, if done correctly, never have your passwords cracked either.

Password Managers come in several models and types, which may suit you better than others. You should try a few out before deciding on one. Keep in mind their limitations as well as their strengths during your choice. Just avoid using the ones that aren't Open Source.

Finally, your password manager can do a little more for your security than just storing passwords. You can store MFA Secrets, PassKeys and other metadata that helps secure your online accounts. Just be sure to back the password vault up routinely to ensure you'll never lose a password!

----

I hope I convinced you to start using a password manager right this moment, and answered any questions you had about them. As I wrote, it's not more difficult to use them, just a little different. With time and practice, I'm sure you'll be used to them and never again have to worry about your passwords. But as usual, [let me know](/contact) if you have any questions as to Password Managers, and I'll update this article to match them!

----

Essay originally published February 24, 2025.

*Opinions are my own and do not necessarily reflect those of my current or former employers*
