A Layman's analysis of Custom Clients wrt. The Information Technology Act, 2000

Tldr; *Is hacking an app somebody else made, running on your own computer, a cybercrime? What about scraping, reverse engineering, and spoofing towards a network API to make an alternative client for it? What about systematically circumventing anti-scraping, anti-reverse-engineering, and iterating on spoof detection technology to avoid a technical ban for exactly that alternative client usage?*

There are 3 angles used by companies to justify TPM:

1. Cybercrime
   
   1. Anti-scraping
   
   2. Fair use policies
   
   3. network ratelimits/anti spam protections
   
   4. The operator's right to final-say over network access methods

## The relevant laws

### Section 43: Penalty and compensation for damage to computer, computer system, etc

If any person <mark>without permission of the owner</mark> or any other <mark>person who is in charge of a computer, computer system or computer network</mark>

1. <mark>accesses</mark> or <mark>secures access</mark> to such <mark>computer</mark>, <mark>computer system</mark> or <mark>computer network</mark> or <mark>computer resource</mark>

2. <mark>downloads</mark>, <mark>copies</mark> or <mark>extracts any data</mark>, <mark>computer data base</mark> or <mark>information</mark> from such computer, computer system or computer network <mark>including information or data held or stored in any removable storage medium</mark>

3. <mark>Introduces</mark> or <mark>causes to be introduced</mark> any <mark>computer contaminant</mark> or <mark>computer virus</mark> into any computer, computer system or computer network;

4. <mark>damages</mark> or <mark>causes to be damaged</mark> any computer, computer system or computer network, data, computer data base or any other programmes residing in such computer, computer system or computer network;

5. <mark>disrupts</mark> or <mark>causes disruption</mark> of any computer, computer system or computer network;

6. <mark>denies</mark> or <mark>causes the denial of access</mark> to any person authorised to access any computer, computer system or computer network by any means;

7. <mark>provides any assistance</mark> to any person to <mark>facilitate access</mark> to a computer, computer system or computer network <mark>in contravention of the provisions of this Act, rules or regulations made thereunder</mark>;

8. <mark>charges the services availed of by a person</mark> to the account of another person <mark>by tampering with or manipulating</mark> any computer, computer system, or computer network;

9. <mark>destroys</mark>, <mark>deletes</mark> or <mark>alters</mark> <mark>any information residing in a computer resource</mark> or <mark>diminishes its value or utility</mark> or <mark>affects it injuriously</mark> by any means;

10. <mark>steal</mark>, <mark>conceal</mark>, <mark>destroys</mark> or <mark>alters</mark> or <mark>causes any person to</mark> steal, conceal, destroy or alter any <mark>computer source code used for a computer resource</mark> <mark>with an intention to cause damage</mark>

For the purposes of this section:

1. “computer contaminant” means any <mark>set of computer instructions</mark> that are designed
   
   1. to <mark>modify</mark>, <mark>destroy</mark>, <mark>record</mark>, <mark>transmit data or programme</mark> residing within a computer, computer system or computer network; or
   
   2. by any means to <mark>usurp</mark> the <mark>normal operation</mark> of the computer, computer system, or computer network

2. “computer data-base” means a <mark>representation of information, knowledge, facts, concepts or instructions</mark> in <mark>text, image, audio, video</mark> that are <mark>being prepared or have been prepared in a formalised manner or have been produced</mark> by a computer, computer system or computer network <mark>and are intended for use in</mark> a computer, computer system or computer network

3. “computer virus” means any <mark>computer instruction</mark>, <mark>information</mark>, <mark>data</mark> or <mark>programme</mark> that <mark>destroys</mark>, <mark>damages</mark>, <mark>degrades</mark> or <mark>adversely affects</mark> the <mark>performance</mark> of a computer resource or <mark>attaches itself to another computer resource</mark> and <mark>operates when a programme, data or instruction is executed</mark> <mark>or some other event takes place in that</mark> computer resource;

4. “damage” means to <mark>destroy,</mark> <mark>alter,</mark> <mark>delete</mark>, <mark>add</mark>, <mark>modify</mark> or <mark>rearrange</mark> <mark>any computer resource by any means</mark>.

5. “computer source code” means the <mark>listing of programme, computer commands, design and layout and programme analysis</mark> of computer resource in <mark>any form</mark>.

#### Commentary

If you do the following without owner/operator permission it's a crime:

1. Does this include engineering, creating, and using a custom client for accessing a computer network, while otherwise respecting its' basic functionality?

2. Does this include a custom client scraping or downloading data from a computer network that "thinks" it's an official client?

3. No comment

4. Is it considered "damage" if a custom client writes data back to the server, in a manner otherwise equivalent to what an official client would do? (or in a potentially novel, if slightly exploitative and unintended manner)

5. No comment

6. No comment

7. No comment

8. No comment

9. Is it destruction or alteration of valuable information, if you continually spoof your client's data in order to stop tracking or personal information from being accurately sent back?

10. This requires a clarification of the definition of "damage" developed above.

### Section 43A: Compensation for failure to protect data

Where a body corporate, possessing, dealing or handling any sensitive personal data or information in a computer resource which it owns, controls or operates, is <mark>negligent in implementing and maintaining reasonable security practices and procedures</mark> and thereby causes wrongful loss or wrongful gain to any person, such body corporate shall be liable to pay damages by way of compensation to the person so affected.

#### Commentary

A company could use this clause to argue that the act of engineering and utilising an (incidentally anti-consumer, anti-competitive, anti-creative) elaborate TPM system with opaque technical lockouts was necessary for maintaining security. The "security" excuse for everything.

## My commentary

I see a few broad issues:

1. It is unclear whether using an alternative, unofficial, or banned method to access a computer resource (e.g a server, social media website's unofficial API, etc) is illegal, if it's not done in order to spam or DDoS the computer resource, or attack its' other users or operator. The text of the statute fails to clarify any notion of user intention or user rights.

2. It is unclear whether the mere fact that an *unofficial* client is accessing a computer resource is enough to say that the other users of the resource are having their privacy violated by the unofficial client. If the user was using an *official* client, the computer resource would otherwise freely and publicly permit the access of user data (e.g users' posts, profile pictures, stories/statuses, direct messages, etc) as according to its' stated and promised function. When you run the Instagram website, it's not a privacy violation for others, but when you run a hypothetical vibecoded MacOS Desktop instagram+BlueSky combined client to download the photos your friend shared you, it's a privacy violation?

The over-collection of bot or client signals to determine whether a client is official or unofficial may itself be a severe violation of privacy and consumer rights, and overly ties the client and server together in an intentionally anticompetitive manner.

Here, a notion is developed that ownership of the program and data belongs only to the person owning or operating the computer resource, and that users may have several restrictions placed on them on what they can and cannot do. (Notably, server operators do not have the restriction placed on them that they mustn't discriminate against users on the basis of what client they're using.) The notion of user rights never enter the picture (i.e user access is suspicious by default, and may only be admitted according to the policy of the operator.)

Obtaining and utilising *unauthorised* access to a computer network is a crime. This is unambigously a legal threat to custom client users. The other clauses don't look friendly either. This requires more contemplation.

# Philosophical Notes

### Punishment and Deterrence for Jailbreaking

One of the most cruelest and effective methods to deter users from jailbreaking your social media app to block your creepy ads is to simply ban their accounts, IP addresses, content, and device fingerprints from your social media server. Users might stomach an ad-blocking client that breaks for a day while the client developers and the server administrators play their cat-and-mouse game, but they will absolutely be unable to handle getting their own accounts banned. Due to platform lock-in, users are often significantly attached to being able to contact their friends, family, colleagues, etc on the network, they literally cannot afford to lose their account or their life falls apart. So companies hold their entire digital presence hostage: if you try and break our unstated rules, we'll cut you off from everyone.

For example, I'm not even able to run WhatsApp on my phone, because it uses GrapheneOS, and my account once got banned for accidental spam years ago. To this day, the WhatsApp server (or client, not sure) somehow thinks that the combination of me running their app on an "unofficial" operating system, and using an account with a "prior history" of policy violation is enough to justify me being unable to access WhatsApp. So, I keep a dedicated old phone for running WhatsApp and lug it around with me everywhere, just to be able to communicate with people. All this in India, where practically all messaging is done through the WhatsApp network! It lets WhatsApp flex its' power to me; If I ever somehow piss WhatsApp off enough to get them to ban me permanently, I'd be completely cut off from my fellow college students, extended family, friends, and colleagues.

(You could say I should just drill down, decompile and jailbreak the app, keep up with the cat and mouse game forever. Or that maybe I should somehow get every single person I know to migrate all of their chats, groups, and organisation to Signal, Matrix, or XMPP. But those are exceedingly hard to do (I've tried, and it's hard because then everybody would have to do it to the next guy!), and somewhere along the way you've forgotten that it was never my responsibility to deal with, solve, or work around the problems that other people actively create. In talking personal responsibility, you've neglected to hold the exact offenders and tyrants responsible for their own crimes, which require all other people to adjust to them in the twisted version of personal responsibility, where people are expected to silently sit and accept whatever happens to them and passively adapt, rather than understand who's really at fault is upstream. This is not a natural disaster or a meteor strike where you technically do not possess the capability to solve the root cause; there is a named company run by living people, individually and collectively, who are the ones setting the conditions for this, and an enshittogenic policy environment that permits this kind of behaviour to begin with.)

What could be done about this? For starters, an analysis of user rights to their account access would be good. Perhaps it would rely on analysis of the DPDPA.

### The consumer rights/digital commons argument for normalising hacking everyone, everywhere, all at once

It's already trite to mention how modern software no longer just works on its own, but architecturally requires a connection to a mothership server in order to do anything at all it's advertised for. Consumers recieve a mere dumb terminal, and the server is where the "interesting things" happen.

Naturally, some consumers don't like this state of affairs, for various reasons of their own. For example, their device may be too old to support the modern apps and they don't want to spend money to obtain a newer compatible device, they may want greater control over their content consumption experience (e.g custom filters, feed orderings, alternative UIs), or they may want to evade surveillance and tracking that the official app forces onto them. One of the ways users have fought back against platform abuse is to make custom **client** applications that connect to the server, and act just like the normal app, while secretly removing or modifying any content according to their wishes, for example blocking ads or trackers. The server unwittingly works with the custom application and just sends away data. This worked for a long while, from the 1990s all the way until the mid 2010s, when centralised social media started wising up to the facts and bolstering their networks or official clients in order to detect modification and ban the user as a lesson to others. Examples of "dumb" custom clients would be [Ripcord](https://cancel.fm/ripcord/), a Discord client, and [Prav](https://prav.app/), an XMPP client. In the case of the proprietary Discord network, Ripcord was created by reverse engineering the Discord Web App, capturing its network communications, and creating a separate program to spoof it, such that it can act exactly like an alternative method of access to Discord. In the case of Prav, XMPP is an open-standard that publishes their technical network communication standards openly on the web, allowing people to create custom clients on their own with far less hacking work. Ultimately the end result is the same: these are alternative programs for accessing a network resource, which may or may not have been originally designed or sanctioned by the network resource's administrator.

Another form of network escape is a **Bridge**. A bridge is a program or code-library intended to connect one disparate network resource to another. Sometimes these may be created between two open platforms, e.g Matrix, XMPP, or Telegram, which publish their network architectures, and provide official, fully feature-complete affordances for programmatic access (or in some cases, simply choose not to punish unofficial programmatic access).

However the interesting bridges are those intended for proprietary platforms such as WhatsApp, Discord, X, etc. Typically these bridge programs may utilise official or unofficial means to map and access the network resource's API, again utilising tactics such as reverse-engineering, scraping, brute-forcing, TPM circumvention, ratelimiting, and fingerprint spoofing to work. When a bridge is published, the public often utilises this to create [new custom clients for accessing those resources](https://github.com/lugvitc/whats4linux), either for personal preferences, or to be able to access network resources from [devices](https://github.com/commandcontrolQ/webbedcord) or [operating systems](https://github.com/DiscordMessenger/dm) that no longer support modern official access methods, or to connect two networks together by directly duplicating their content to one-another, or [translating them to their respective forms using their respective programming conventions](https://fed.brid.gy/), live. Ultimately this is the technical realisation of the intention behind Section 52(1)(ab) and (ac): the doing of anything necessary to interoperate two independent programmes, and the study or test of a programme in order to ascertain its' function in order to do just that.

Today, software such as Instagram, WhatsApp, etc contain highly complex TPMs that have one purpose: detect if the user is using an unofficial client or API wrapper, and block them if they are, or permaban their accounts for deterrence. Detecting and deterring jailbreaking is itself one of the major areas of investment in user-facing technology, because given the opportunity the majority of users would *gladly* jailbreak and circumvent *the shit* out of all their tech to escape corporate abuse and spying *en masse*.

Here is the fundamental tension between the user-rights side and the internet-freedom side:

the operator-rights side:

1. The operator is not obliged to provide any amount of network resource access to anyone, including current or prospective users. They may provide and withdraw access at their discretion, with or without explanation of cause. (This is what allows operators to protect "normal" users, by quickly banning spammers, hackers, or data breachers.)

2. The operator is not obliged to adhere to the users' wishes or demands that a specific feature be added, modified, or removed in any way. (This is what allows operators to implement and strengthen any anti-circumvention or content moderation technology they want, and restrict user accessible functionality arbitrarily.)

The user-rights angle, meanwhile, calls on two things:

1. Users must have some rights as consumers and data principals that trump the EULA they sign with a network resource operator.

2. Technically, users are able to access any internet resource by any means it is technically possible to do so, no matter the wishes or business model of the operator. This is due to the underlying nature of the internet as a fundamentally open and highly interconnectable system.

The relationship between these two parties is governed by the EULA. In case such a restriction within the EULA is not enforceable, the same may be backstopped by calling upon Section 43A.

While the contention between public creativity and statutory monopoly under Copyright law is clear-cut in India, the same is not for cybercrime. There are 4 other angles that need to be looked at:

1. Data Privacy (DPDPA)

2. Competition (Competition Act)

3. Consumer Rights (Consumer Rights Act)

4. Trade Secret Violation
