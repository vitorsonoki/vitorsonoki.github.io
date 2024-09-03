# An interesting French letter-based scam

Outline:

 - The "Lecoq" premium letter based scam.
 - They take your IBAN and credit card number and sign you up for a bunch of services they presumably have affiliation bonuses with. After collecting the bonus, you're left with a bunch of unwanted paid services that you have to cancel.
 - Explanation: https://www.signal-arnaques.com/scam/view/442551#comment-1422246 (in French).
 - If something is too good to be true - it probably is.
 - "Your data is safe with StarData SAS" - most meaningless comment ever in a scam.

I can't believe what I'm seeing. Me? The rightful, legally appointed receiver of 5000 Euros per month, free of tax, for the next twenty years? And all I have to do is call this phone number?

Such was the promise of a letter - in fact, a *personal* letter, addressed to my wife and marked as "confidential" - that we received in the mail a few weeks ago. It's in French, presumably intended for a French audience, and that oozes with assurance that you can trust the sender about his magnanimous intentions of issuing you with what's basically a free income for the duration of your productive lifetime.

That sender has a name, too, Monsieur Emmanuel Lecoq, who signed it in blue pen and included his organization's (COAP) official seal. That organization has a name and address in Paris, and under their commitment to data safety, they guarantee that all your information will be safe under the steward of "StarData SAS," a company headquartered in Paris's 5th Arrondissement. And to guarantee that this letter is really for your eyes only, M. Lecoq includes a set of personal credentials, essentially a username and password, that only you can use to prove your identity and claim the money. Legit, right?

As usual, if it sounds too good to be true, it probably is. Three minutes into reading it, I was ready to shred the letter and chuck it into the trash, but I stopped, because even this ridiculous, obviously fake scam gives us some interesting material to explore. For example, what could go wrong? What are the criminals behind this scam looking for? How do they bait and profit from your actions? 

Those are all interesting points of information that we can study to better understand and prepare against similar future scams. Let's see in depth.

## How does this scam progresses

The universal best way to find out how a scam works is to just search for the elements that compose it. For example: the setup, the premises, the things that are sent or informed to you as bait, etc. This is because save for some very rare situations, you will not be the only one targeted in a scam attempt, no matter how personal it might seem. You will find other people who faced or, sadly, fell for it.

Doing this in a less familiar language may be more challenging, but after a few searches, I was able to catch wind of how this scam works. The premises change a little from case to case, like the amount of money involved, the payment scheme (large amount of money up front or recurring smaller payments) and sometimes the company name, but the activities "behind the scenes" are always done in a similar manner. Interestingly, the one thing that seems to remain a constant is the mentioned name of Emmanuel Lecoq. Talk about a determined attempt to keep his name legit!

In this scam, the mark (victim) is requested to call a phone number in the letter to claim the reward, and prove their identity by supplying them the two "secret" numbers contained in the letter ("Combinaison" and "code personnel"). While these two numbers are not really required in the working of this scam as you will see, they still could be used by the attackers to confirm that a certain mark has fallen for it, which can signal them that this mark could be successfully attacked again in the future. 

Behind that phone number there is a legitimate-sounding call center that picks up the call and begins by "confirming" the identity of the mark and congratulating him/her on the chance. In order for the "benefits" to be sent successfully, the scammers say, they need some financial information from the mark, specifically a bank account number (IBAN). Standard procedures, the mark might think, but then they deepen the request by asking for a Credit / Debit card number. At this point, the mark could get suspicious regarding the request, but the scammers assure that this is an additional layer of verification, required to cross-check that the information being provided is correct. 

As the mark passes this information, the scammers may ask for it again ("I'm sorry, I didn't quite get it, could you repeat? Are you sure that your IBAN is ABCDE...? Oh, my mistake, I thought you said ACDE...") or place the call briefly on hold for purposes of "verification." In reality, there's absolutely no verification or system time being used at all - the scammers are just using this as a way to buy time for themselves.

After a long string of "verifications," the operators suddenly announce that all the information matches and thanks the mark for bearing with them all this time and that they will be getting in touch back with them later, and the call is over.

As strange as this scheme went, with a long verification process, call centers and a seemingly legitimate combination of ID number and password, if you reached that point of hanging up, it's too late already. *The scam is already over* and the scammers have already run away with their profits. So what just happened here?

## How the scam works

To dissect the scam, we just need to back to the time when the mark is asked to submit and verify his / her information. During that phony "verification" phase, the scammers already are in posession of two pieces of financial information: the mark's IBAN and bank card number. Although there's not a lot of "exfiltration" risk that one can have by simply crossing those two, indeed, there's another very popular way that those two are used in Europe, and for which there's indeed very little security verification that goes on: automatic debit via the [SEPA](https://www.inkle.io/blog/understanding-sepa-transfers-a-complete-guide) system.

As they waste the time of the mark by repeatedly performing "verification" of his information, in the backstage, the scammers are actually plenty busy. They are using the mark's information to sign up to as many online services with recurring payments as possible, *setting up many SEPA direct debits* in the process. What online services? Gaming subscriptions, streaming platforms, computer "security" subscriptions, anything with a monthly fee. Note, however, that not a single one of these services are owned by the scammers. So if they're not getting the money being charged to the mark, what do they gain with this?

The answer is *commissions*. The scammers already have arrangesments with these services so that they can earn a commission every time they close a "sale" of a new subscription, much like in the sprawling world of affiliate marketing nowadays on the internet. Those service providers apparently care very little on how the "sale" itself was conducted - marketing? Suggestion? Coercion? Scam? Who cares, it's more money!

The scammers buy more time for their works by pretending to keep validating the information from the mark and keep him busy (so he won't look into his bank's statements or other alerts that could fire from this activities), while milking for more of these commission fees of garbage services. So by the time they hang up, it's already too late; the mark is already "signed up" for dozens of those useless services and the scammers parted with their share of profits, scraped off of many unsuspecting (and legitimate) affiliate and commission-based programs.

Note that this is a *lot* more interesting for the scammers than the other possibilities that the scenario could take. If they attempted to use that SEPA debit capability to siphon off the mark's money to themselves, they would have to disclose a bank account under their possession, opening themselves to a fraud investigation by the bank which would be easily traced back to them by the police. If they used the information to make fraudulent purchases for themselves via the mark's card or bank, this again could be intercepted via fraud monitoring and the scammers traced back as well. 

By reducing the activities to the relatively simpler commission-signing up, the scammers get exposed a lot less to either party, and can probably continue doing so for long until a suspicion arises. No hacking is required, no information from the scammers is exposed. The only downside is that the gains are reduced to what is paid via commission fees.

## How are people targeted?

It's clear that the scammers behind this scheme do a fair amount of research and are targetting a specific demographic of France, given the preparation in sending individual letters, complete with tracking numbers. While I couldn't validate it, my theory is that the target population for this scam is the poor people looking for benefits or employment via the French Government's *Pôle Emploi* agency.

About a year earlier, my wife was advised to register with that agency to state her then-unemployment and receive some job opportunities. This involved the exchanging of some personal information, including an address, to be registered in the platform. And even though nothing came out of it, this narrows down the possible causes, because out of all the services - goverment or not - that we had to register in France, the Pôle Emploi is the only one for which only her signed up for without me.

This indeed makes sense for a scam: after all, poor people looking for jobs or benefits are more likely to be desperate to "earn" money quickly and not verify sources. So, sadly, again the poor population bear the brunt of greedy scammers. However, another interesting question arises from this point: if a government agency is entrusted with protecting the data it needs to work, how did this very data end up in the hands of criminals?

For starters, I'd discard the possibility of a *data leak* in the agency originating from a hack in their systems. Judging by the amount of reporting going around, this scam has been happening for a few years now, and if the data was leaked only once, it would probably be stale by now (the scammers would have run out of victims). Finally, data breaches such as this tend to gather large media attention in the security circles, would have to occur in a regular basis for this to happen (since my wife registered just the year before she was targeted). It's unlikely it happened this way.

That leaves us with the other possibility: that a *malicious insider* with access to those databases has been collaborating with the operators of this scheme. This would be a lot easier on the scammers' side: no hacking would be required, no risk of being caught, and the only cost is a small cut in the profits, paid under the table to that collaborator. That insider in a priviledged position can just siphon off interesting information, new victims, or the whole thing to the attackers in a periodical basis, enabling the scheme to continue year after year.

It wouldn't be the first time that I've seen this malicious collaboration, either. In Brazil, I witnessed an ISP attempt to scare a customer into not switching away to another provider by robo-calling him about a fake service fine related for doing so.

## How to protect yourself

As usual, the old adage of "prevention is better than the cure" applies here. If you were targeted by some campaign like this, learn how to identify the usual catch handles of such scams: a high reward, attempts of endearment or a special bonding, an overall sense of urgency or pressing ("if you don't act now, then...") and the feeling of "too good to be true." If you steer away from it before it even begins, you avoid it completely.

If you already find yourself in the middle of the scam attempt, stop and buy yourself some time to *rationalize*. Is what's being promised (or threatened, in the case of a "scare" scam) really possible? What are the odds? How can I know that the person on the other side really who he or she says they are or even a person at all? Stash away the feelings, put the rational brain to think. 

Most importantly: give yourself *time* to stop and think and refresh the whole situation. Nothing of real importance here can't afford to wait - it's only the scammers' pressure that makes it seem so. Just giving yourself time to breath and distance yourself from the conversation should be able to give you some vantage point from which you can see how the scammers' threats or rewards are so unrealistic or pointless.

And if this sort of scam unfortunately has *already* happened to you, check all your bank accounts immediately and cancel the card that has been compromised. Check the automatic debit statements that have been added; most online services make use of a few days' grace period during which they may be cancelled free of charge. Cancelling things may not be the easiest task around (everyone puts hurdles to "persuade" you otherwise), but it's always on your right and should be doable before that grace period.

## Conclusion

Scams like this will not go away any time soon. Not when there's a growing supply of new potential marks coming out every year (France's Pôle Emploi is a popular destination for youths right off high school), and where the rewards outweight the risk. And sadly, while this "insider" operating the inner half of the scam doesn't get ousted by the goverment agency, this and similar schemes may continue unchecked for many more years.

A good critical analysis of risk vs reward, combined wiht a rationalization of the feelings of greed and urgency can prove to be vital to avoid falling in this net completely. But where those cannot be applied (think of cases where the mark is "warmed up" via other channels to make him/her more likely to fall), active monitoring of your finances can be useful.

I personally think there's something quite messed up with the how easily SEPA automatic debit transfers can be set up in such a fraudulent manner as this one. Granted, [banking has vulnerabilities pretty much anywhere in the world](https://security.stackexchange.com/questions/6598/can-someone-steal-money-from-my-bank-account-if-they-know-my-iban-and-personal-d), but the way it's set in Europe really seems to make it too easy. An IBAN - essentially a bank account number - is not by any means a secret, and for organizations, might as well be considered public information. After all, how otherwise could you receive money? And even though credit card numbers might be thought of as more sensitive, the truth is that they are not nearly as well protected as true secrets such as passwords, and are often transmitted in the clear, even spoken out loud between two people over a phone call.

So basically, all it takes to get a bank to transfer money out of a client's account is these two non-secret pieces of information, one of which might as well be found in a quick internet search, and the other can probably be found with some diligent OSINT work. No more questions asked! And nowhere in the process is the client ever inquired ("are you sure you wanna do this? Is this really you?" Etc). I would say that this is a seriously lacking point in the European banking systems.

While this system doesn't get reformed to patch this weakness somehow, a regular monitoring of your accounts and finances is your next best bet. How often do you check your accounts? Do you know exactly how many and which services get billed to you automatically? Reviewing these in a regular basis is useful, and if you can change some for you to pay proactively can be even better (it would also give you an opportunity to review whether you still really need them).

And as always, stay safe out there in this scammers' world!

----

Source for the [explanation of the scam](https://www.signal-arnaques.com/scam/view/442551#comment-1422246) (en Français).

----

*Opinions are my own and do not necessarily reflect those of my current or former employers*
