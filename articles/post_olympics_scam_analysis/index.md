# Post-Olympics scam analysis

<figure>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9e/Le_concours_international_de_p%C3%AAche_%C3%A0_la_ligne_%C3%A0_l%27exposition_universelle_de_1900.jpg/521px-Le_concours_international_de_p%C3%AAche_%C3%A0_la_ligne_%C3%A0_l%27exposition_universelle_de_1900.jpg" alt="Angling at 1900 Olympics at Paris" />
    <figcaption>
        Believe it or not, but fishing (referred to by its street name "angling") <a href="https://en.wikipedia.org/wiki/Angling_at_the_1900_Summer_Olympics">was once an Olympic discipline</a> in 1900. Credit <a href="https://en.wikipedia.org/wiki/File:Le_concours_international_de_p%C3%AAche_%C3%A0_la_ligne_%C3%A0_l%27exposition_universelle_de_1900.jpg">Wikimedia</a>.
    </figcaption>
</figure>

The day is August 12, 2024. 

Just the day before, the world watched in awe the closing ceremony of the Games of the 33rd Olympiad in Paris and the iconic Olympic flame was extinguished, marking the official end of the games.

Today, less than 24 hours after that ceremony, however, something interesting happened in my wife's Instagram feed - an ad served smack dab in the middle announcing sales with a huge discount in Olympics and Paris 2024 official apparel. And when I say discount here, I'm *really* talking discount - I'm talking €35 t-shirts selling for €7 kinds of discounts. It said right there in the ad. Surely my wife and I wanted something like this. I mean, what better way to get Olympics' memorabilia than at a bargain sale? Sweet deal, right?

Except for one thing: Paris 2024 also does the *Paralympics* like every other organizing committee since 1988, which means that any serious sales will not really start until at least another month or so after the Olympics. Which in turn means that particular ad was yet another indiscriminate *scam attempt*.

In the daily life of the largest single event of the world, one more scam or phishing attempt is just business as usual. Everyone knows these happen - or at least should - but one department that is always aware of them is Information Security. Here's the thing, though: even you don't work on it, you should act like your own. Dealing with these non-technical, yet tricky scam and phishing attempts are something that you should cultivate as part of your own digital self-defense skills.

So as part of an educational series and also honing in my own self-defense skills, I'll break down this scam / phishing attempt.

# The bait

Sadly, I do not have an image of the ad in question that was served through my wife's feed to share. And at this point, I believe moderation efforts coupled with a few times flagging that ad as scam have already removed all traces of it and the associated account from Instagram.

However, the very fact that that ad was *allowed* to exist for a few hours or even days in Instagram with no prior background checking is worrying; in a world full of uncertainty and fabricated information on the internet, these scammers were able to pay for and get a window of time to do their dirty business *legitimately* in what's probably the world's busiest platform. Shame on Meta for allowing this to exist while shamelessly ban-hammering a bunch of other unoffensive content.

This is the link behind the ad, with some sanitization:

    https://www.olympicsvipshop [.] com/?fbclid=PAZXh0bgNhZW0BMAABprq1aMK...(a long tracker)

Ah, yes, `olympicsvipshop[.] com`. If this attempt is not evident by now, let's break it down a little further.

For starters, the International Olympic Committee uses the domain `olympics.com`, and Paris 2024's own website is built into it as well. The same goes for the official store - built into `olympics.com`. In fact, anything official from the IOC or the editions of the games at this moment is hosted under that domain - period. 

That alone should stop you from doing any further business with this so-called "VIP shop," but if we need even more evidence, let's get a little technical:

A simple `whois` query to the shady domain reveals some interesting metadata:

    Domain Name: OLYMPICSVIPSHOP.COM
    Registry Domain ID: 2907401950_DOMAIN_COM-VRSN
    ...
    Updated Date: 2024-08-13T02:53:17Z
    Creation Date: 2024-08-12T15:27:07Z
    ...
    Registrar: Cloud Yuqu LLC
    
Right. So this "VIP Shop" magically is created by someone in China the day after the Olympics, and it already is promising us a bunch of miraculous discounts. Must be really the official source, huh!

There's more fishy stuff, though:

    ...
    Registrant City: REDACTED FOR PRIVACY
    Registrant State/Province: BeiJin
    Registrant Postal Code: REDACTED FOR PRIVACY
    Registrant Country: CN
    Registrant Phone: REDACTED FOR PRIVACY
    ...

Last time I checked, [Beijing, China](https://en.wikipedia.org/wiki/Beijing) is written with a 'g' in the end, and `BeiJin` is not part of any of the [names given to that city in other languages](https://en.wikipedia.org/wiki/Names_of_Beijing) either. 

Also I can't help but think how funny it is to see how so much stuff has been `REDACTED FOR PRIVACY` by the registrar, and yet the most obvious pieces of information are left in the open, and even under a typo. How professional!

If these by now *still* have not raised multiple red flags for you, though, fret not. We can go a step further - into the monster's lair.

# The platform

<blockquote class="warning">
    <strong>Disclaimer:</strong> do NOT attempt the procedure below unless you are versed in forensics or IT Security and know how browsers and exploits work.
</blockquote>

After we put on a digital condom (a sandboxed browser, virtual machine or a text-only browser with no javascript plus a proxy), we can finally visit how this `olympicsvipshop [.] com` website and see it for ourselves what it really is about. What horrors lie beyond that crappy domain? Malware hosting? Exploits? Phishing site?

As it turns out, nothing really. Just disappointing, half-baked stuff that not even a kid with a Wordpress installation would deliver:

![home page](/static/olympicsvipshop_home.jpg)

There's nothing even "Olympic" about that website anywhere. And what up with that word "best" just hanging in there for a lack of a title? How half-assed can these guys get!

I tried to even search something related to see if the scam goods of the old ad would show up again but, alas, nothing.

![search page empty](/static/olympicsvipshop_search.jpg)

The contact page was done with a little more effort, but the amount of broken English and downright copied-and-pasted pseudo-marketing lingo contained in there is stuff of comedy:

![contact page](/static/olympicsvipshop_contact.jpg)

That email address is a dead end, by the way. The domain `clientreplycenter [.] com` is at this time parked by Hostinger and nothing is hosted in there. It's just a bait and switch intended to infuriate you even more after you write a long angry letter demanding a refund to that "customer service" email, only to find out that the address does not exist.

![parked page](/static/olympicsvipshop_parked.jpg)

There is, however, one more interesting nugget in there: the address **Weggisgasse 13, 704 Luzern, Switzerland** where this store is supposedly based. Turns out this is indeed a real address in Switzerland - but it actually belongs to a United Colors of Benetton store:

![osm print](/static/olympicsvipshop_address.jpg)

I'm sure that Benetton would love to know how people scammed online are being directed to their store for complaints and demands of refund. And to save the best for last, I finally lost it in the "about us" page - they can't even agree on what is the name of the company in the end!

![about page](/static/olympicsvipshop_about.jpg)

# Conclusion

This scam site showed up all the obvious signs of what a scam site looks like so it was too easy to analyze. But the methods used here remain valid and you should familiarize yourself with them. After all, today this is just one domain with a hastily done crappy site, but what about in a few years? Someone could re-use this same domain and attach it to an actually dangerous malicious server later on, serving malware to unsuspecting visitors. Don't underestimate what criminals can do on the internet!

This is why the first steps in identifying a scam or phishing site are so important - the best way to avoid the hack is to steer away from it *before* it happens. Does it look "too good to be true?" Perhaps urgent? Suspiciously personal from someone who wouldn't otherwise write to you? Grain of salt, doubt and verify the source through a different channel - how about calling the person who supposedly sent that suspicious email?

Finally, we have to re-think the concept of not trusting "different URLs." I'm talking about the concept where users are given a set of "official" URLs (usually the company intranet and domains) and told not to trust or even consider anything else. Although this concept is still valid a lot of the time, this is not a panacea against phishing or similar attacks and I don't think it should be used like so.

Consider Paris 2024. The organizing committee itself has changed the address for its official website (originally Paris2024.org, now taken under the IOC website) and even the IOC did so (from a `.org` to a `.com` domain). How can users keep following a chain of changes to formerly "trusted" domains? If anything, this is additional load given to the IT Service Desk who has to keep answering those "is this safe? Can I click this link?" kinds of questions.

Now add to this mix a couple of different collaboration tools sourced from third party suppliers, like a new Sharepoint site, some project tracking platform, etc, all coming with entirely new unknown domains because we don't wanna pay extra to this SaaS. Finally, let's not mention when people start sharing links from those "free online tools" to do things like as trivial as deciding a common date and time for a happy hour, and you can see how the strict concept of "trusted URLs" really goes out of the window. I'm not saying this is entirely outdated or not usable, but there must be a better way to educate users on this.

And lastly, if you're still wondering about getting a good discount in Olympic Apparel, remember this: Paris 2024 goes all the way to the Paralympics. Those prices in the store will probably do so to.

---

Essay originally published August 18th 2024.

*Opinions are my own and do not necessarily reflect those of my current or former employers*
