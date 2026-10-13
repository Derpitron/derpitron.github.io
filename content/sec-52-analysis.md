# A Layman's Analysis of Section 52(1)(aa)-(ad), Indian Copyright Act, 2012

Tldr; *Can software EULAs take away or legally restrict your precious Sec.52(1)(aa)-(ad) rights? Probably not, but nobody's sure.*

This is my unqualified interpretation of Indian Copyright Law with a focus on software user rights. I highlight some terms in the clauses that I found interesting and concerningly poorly defined/tested, and raise a few nitpicky/conceptual doubts I've developed over the months and haven't found satisfactory answer to. This builds on me, 28LiterMicrowave, and Akash's research and analysis in [Beyond Copyright Enforcement - Technological Protection Measures and User Rights in India](https://28litermicrowave.com/paper.pdf) to give a slightly more targeted, direct interpretation.

I've searched the internet for months for precedent regarding Sec.52(1)(aa)-(ad), but haven't found any. As far as I can tell, there is no clue yet how narrowly or broadly, pro-Big Tech or pro-user the courts would interpret it.

Here, I try to make a **copyright maximalist interpretation**, as a sort of "worst case" scenario of legal gaps that I think the Indian FOSS community, digital rights activists, consumer rights activists, or antimonopoly activists may face if they take up these things in court. If anybody has any info invalidating my interpretation, please reach out to me and I'd love to hear it and publish it here. If you think all of this is naive or gravely misinformed pedantry, I'd also love to hear about that too!

In the future, I also wish to examine where exactly the exercise of Section 52 rights may conflict with *The Information Technology Act, 2021*'s anti-hacking/cybercrime-related clauses, and potentially investigate scenarios where common right-to-repair/interoperability actions may be permitted by Section 52 (in both the pro-Big Tech and pro-user interpretation) but run afoul of those laws. I wish to also provide my own severely unqualified broad, pro-user interpretation of the Section 52 rights, alongside a pro-Big Tech interpretation. Doing this might spread awareness of the fact that what we commonly think are morally/legally grey actions today (e.g game modding, jailbreaking, decompiling) might be entirely within users' rights.

I am not a lawyer nor is any of this legal advice. I'm a humble independent observer and mere citizen of the nation pls dont sue me :pray:

## The Relevant Laws

### Section 14: Meaning of copyright

For the purposes of this Act, copyright means the <mark>exclusive right</mark> <mark>subject to the provisions of this Act</mark>, to <mark>do or authorise the doing of any of the following acts</mark> in respect of a <mark>work or any substantial part thereof</mark>, namely:

1. in the case of a literary, dramatic or musical work, not being a computer programme,--
   
   1. to <mark>reproduce the work in any material form</mark> including the storing of it in <mark>any medium by electronic means</mark>;
   
   2. to <mark>issue copies of the work to the public</mark> <mark>not being copies already in circulation</mark>;
   
   3. to <mark>perform the work in public</mark>, or <mark>communicate it to the public</mark>;
   
   4. to make any cinematograph film or sound recording in respect of the work;
   
   5. to <mark>make any translation</mark> of the work;
   
   6. to <mark>make any adaptation</mark> of the work;
   
   7. to do, <mark>in relation to a translation or an adaptation of the work</mark>, <mark>any of the acts specified in relation to the work in sub-clauses (i) to (vi)</mark>;

2. in the case of a computer programme:
   
   1. to do any of the acts specified in clause (a);
   2. to <mark>sell or give on commercial rental</mark> or <mark>offer for sale or for commercial rental</mark> <mark>any copy of the computer programmer</mark>[sic]: Provided that such commercial rental <mark>does not apply in respect of computer programmes where the programme itself is not the essential object of the rental</mark>.

For the purposes of this section, <mark>a copy which has been sold once</mark> shall be deemed to be a <mark>copy already in circulation</mark>

#### Commentary:

This section defines what the Copy Rights are specifically. Useful to keep it in mind when the idea of "restricting" or "waiving" copyrights arises later.

 The following questions are unclear, and answering them would demarcate some important boundaries for software.

1. 1. Does "reproduce" mean a (bit-for-bit, bug-for-bug, spiritual) copy?
   
   2. Does this include transferring (code, assets) of a programme to a user's computer?
   
   3. Does this include running (code, assets) for third-party usage on a network, without transferring the same to the user's computer?
   
   4. N/A
   
   5. Does "translate" imply language translation, source porting, or emulation? Does this imply exact preservation of bug-for-bug (functionality, intention, behaviour), or an AST?
   
   6. 1. Does "adapt" include (modification, addition, or deletion) of (content or (intended or accidental) functionality)? What is the test for this?
      2. Is an independently authored, but functionally dependent plug-in, modification, patch, front-end, or program a separate work, or falls under the original work? What is the test for functional dependency and independence of authorship?
   
   7. No comment

2. a 
   
   1. No comment
   2. Does "commercial rental" imply the consumer doesn't get copyright over their own copy?

Is "usage" right of a work (e.g running, using, accessing a computer programme) governed by copyright?

### Section 17: First owner of copyright

Subject to the provisions of this Act, the <mark>author of a work</mark> shall be
the <mark>first owner of the copyright therein</mark>, provided that...

#### Commentary

Does (work, an addition, modification, or deletion of a work) created by a third-party under Fair Dealing (Sec.52) automatically belong to (owner of copyright of the original work, third-party who performed the modification, or the public domain)?

### Section 30: Licences by owners of copyright

The owner of the copyright in any existing work of the prospective owner of the copyright in any future work may <mark>grant</mark> <mark>any interest in the right</mark> by licence in writing by him or by his duly authorised agent: Provided that in the case of a licence relating to copyright in any future work, the licence shall take effect only when the work comes into existence.

Explanation: Where a person to whom a licence relating to copyright in any future work is granted under this section dies before the work comes into existence, his legal representatives shall, in the absence of any provision to the contrary in the licence, be entitled to the benefit of the licence.

#### Commentary

Does the right to grant (copyright, part(s) of copyright) include the right to

1. (condition, waive) any fair dealing rights (Section 52)?
   
   1. No, I think. Section 52 rights, technically, states that some actions aren't copyright exceptions. This means that these actions mustn't fall under any form of copyright regulation. Section 30 does not contain any provision allowing a copyright holder to randomly create new copy-rights where one does not exist, and thereby use that to argue that a user effectively exercising them would then be in violation of copyright. Fair dealing simply cannot be enjoined by copyright.

2. Stop copyright exhaustion on sale, distribution, transfer (under Section 14(a)(ii))? **YES (Engineering Analysis Centre of Excellence Ltd. vs CIT, 2021).** Though this would be weird. The way to stop copyright exhaustion is to restrict users' rights in the EULA to an unknown degree, which the Court would then recognise as taking away their ownership over the copy they physically possess. However, the same restrictions would still be unable to restrict the same conduct if performed under Section 52. (So the same contract clause that takes away your ownership is itself defeated by your Section 52 rights.)

### Section 51: When copyright infringed

1. Copyright in a work shall be deemed to be infringed:
   
   1. when any person, <mark>without a licence granted by the owner of the copyright</mark> or the Registrar of Copyrights under this Act or in <mark>contravention of the conditions of a licence so granted</mark> or of <mark>any condition imposed by a competent authority under this Act</mark>
      
      1. <mark>does anything, the exclusive right to do which</mark> is by this Act conferred upon the <mark>owner of the copyright</mark>, or
      
      2. <mark>permits for profit</mark> any place to be used for the <mark>communication of the work to the public</mark> <mark>where such communication constitutes an infringement of the copyright in the work</mark>, <mark>unless he was not aware</mark> and had no reasonable ground for believing that such communication to the public would be an infringement of copyright; or
   
   2. when any person
      
      1. <mark>makes</mark> for <mark>sale or hire</mark>, or <mark>sells</mark> or <mark>lets</mark> for <mark>hire</mark>, or <mark>by way of trade</mark> <mark>displays or offers</mark> for <mark>sale or hire</mark>, or
      2. <mark>distributes</mark> either <mark>for the purpose of trade</mark> or to <mark>such an extent as to affect prejudicially</mark> the <mark>owner of the copyright</mark>, or
      3. <mark>by way of trade</mark> <mark>exhibits in public</mark>, or
      4. <mark>imports into India</mark>, any <mark>infringing copies</mark> of the work (Provided that nothing in sub-clause (iv) shall apply to the <mark>import of one copy</mark> of any work for the <mark>private and domestic use of the importer</mark>.)

#### Commentary

This paragraph bans jailbreaking, reverse engineering, and modding as commercial activities, meaning they cannot be done for profit. This is quite bad and leaves reverse engineering solely in the hobby/consumer rights territory, while threatening the competitive potential.

1. This section defines copyright infringements.
   
   1. No comment, refer Section 14.
   
   2. Bans commercial public broadcast of copyright infringements

2. This section defines commercial practices that violate copyright. When they bring up "infringing copies", it could mean both verbatim and modified copies.
   
   1. Does "sale or hire" include free(gratis) distribution?
   2. Blocking copyright infringements from prejudicially affecting the owner of copyright could be seen as affecting competition.
   3. No comment.
   4. No comment.

### Section 52: ㅤㅤCertain acts not to be infringement of copyright

1. The following acts shall <mark>not constitute an infringement of copyright</mark>, namely:
   
   1. the <mark>making of copies</mark> or <mark>adaptation</mark> of a computer programme <mark>by the lawful possessor of a copy of such computer programme</mark>, <mark>from such copy</mark>
      
      1. <mark>in order to</mark> <mark>utilise</mark> the computer programme for the <mark>purpose for which it was supplied</mark>; or
      
      2. <mark>to make back-up copies</mark> <mark>purely</mark> as a <mark>temporary protection</mark> against <mark>loss, destruction or damage</mark> in order <mark>only to utilise</mark> the computer programme for <mark>the purpose for which it was supplied</mark>
   
   2. the <mark>doing of any act necessary</mark> to <mark>obtain information</mark> <mark>essential</mark> for <mark>operating interoperability</mark> of an <mark>independently created</mark> computer programmes[sic] <mark>with other programmer</mark>[sic?] <mark>by a lawful possessor</mark> of <mark>a</mark> computer programme <mark>provided </mark>that <mark>such information</mark> is <mark>not otherwise readily available</mark>
   
   3. the <mark>observation</mark>, <mark>study</mark> or <mark>test</mark> <mark>of functioning</mark> of the computer programme <mark>in order to determine</mark> the <mark>ideas and principles</mark> which <mark>underline</mark> <mark>any elements of the programme</mark> <mark>while performing</mark> <mark>such acts</mark> <mark>necessary</mark> for the <mark>functions</mark> <mark>for which the computer programme was supplied</mark>
   
   4. the <mark>making of copies</mark> or <mark>adaptation</mark> of the computer programme <mark>from</mark> a <mark>personally</mark> <mark>legally obtained copy</mark> for <mark>non-commercial</mark> <mark>personal</mark> use

2. The provisions of sub-section (1) shall apply to the <mark>doing of any act</mark> <mark>in relation to the translation of a literary</mark>, dramatic or musical work <mark>or the adaptation of a literary</mark>, dramatic, musical or artistic work <mark>as they apply in relation to the work itself</mark>.

#### Commentary

##### Copyright Maximalist Interpretation

1. The following acts are not copyright infringements:
   
   1. Making verbatim, or modified copies of a program you lawfully possess (but do not have any part of copyright to), in order to
      
      1. Use that copy of the program. But only for the purpose that copy was supplied for, and not any novel, unintended, or contractually restricted usecase.
      
      2. Make backup copies only as a temporary protection against loss, destruction, or damage of that specific copy of the program. But to use those backups only for the purpose the original program was supplied for, not any novel, unintended, or contractually restricted usecase.
   
   2. Do only what is strictly necessary to any software, in order to obtain only the bare minimum information essential for operating the possibility of interoperability of any specifically independently created (i.e clean-room engineered) program with any other program. But only if that bare minimum required information is not already available, in any clear, confusing, or incomplete form, to the actor.
   
   3. The passive observation, study, or test (and explicitly not decompilation, debugging, clean-room-reproduction, or modification) of the readily apparent functioning or effects of the program, to understand how it works. But only if this study is done simultaneously while using the program for the purpose it was supplied for, and not for any novel, unintended, or contractually restricted usecase. (For example, you're not allowed to reverse engineer the weights or training process of a raw neural network program you have on your disk.)
   
   4. Making verbatim, or modified copies of a program you legally obtained (but do not have any part of copyright to) in a personal (and not commercial) capacity, and only for non-commercial (i.e recreational, academic use, not used in the course of employed/contracted commercial gain) and personal (i.e only for you, not for your friend, a small personally known audience, or the public at large) (However, it may be any allowed usecase, including purpose which the program was not supplied for.)

##### Are these Rights, or Decriminalisation?

It is important to understand whether Section 52 provides a *statutory right* to certain conduct, or merely *decriminalisation*. The nature of Section 52 affects people's rights and the remedies they could seek.

> A right would *protect* public conduct, letting people sue manufacturers or developers who technically violate them for a hefty settlement. It would also mean that manufacturers or developers inserting restrictive clauses into their contracts would be *violations of public policy*, and the restrictions would not be enforceable in court, and users could use the "fair dealing" defense in court to protect themselves from corporations in court.
> 
> Decriminalisation would not provide this level of protection. Decriminalisation would merely mean that manufacturers could instead move the ban on hacking to a contract (for example, an EULA or ToS), where it would instead be solely a *contractual violation*, enforceable by the court.

It's important to understand that the purpose of copyright is, first and foremost, to *protect public creativity*, not to stifle it. Further, exceptions to copyright are not merely an "escape hatch" or "loophole", but rather a *vital* part of copyright that ensures that the *public creativity* part of "protect public creativity" can go on to live. Without fair dealing rights, we would only have the "protect" part at the expense of "public creativity", i.e a monopoly. [Several](https://indiankanoon.org/doc/138192511/) [court](https://indiankanoon.org/doc/164343914/) [cases](https://indiankanoon.org/doc/1017103/) [have](https://indiankanoon.org/doc/543688/) [stated](https://indiankanoon.org/doc/93327052/) as much.

[ANI vs. OpenAI](https://indiankanoon.org/doc/93327052/) states:

> 166. The legal principle that emerges from a reading of the aforesaid
>      judgments is that [Section 52](https://indiankanoon.org/doc/1013176/) of the Copyright Act <mark>strikes a balance</mark> between
>      the exclusive rights granted to the owner of the copyright and the <mark>competing
>      public interest of encouraging creativity and disseminating knowledge.</mark>
>      Hence, [Section 52](https://indiankanoon.org/doc/1013176/) is <mark>not in the nature of a proviso or an exception</mark> to the
>      [Section 51](https://indiankanoon.org/doc/1038145/) of the Copyright Act.
> 
> 167. In my respectful view, [Section 52](https://indiankanoon.org/doc/1013176/) independently defines the
>      <mark>rights/privileges of a user in respect of copyrighted works</mark> and <mark>must not be
>      interpreted in a restrictive manner.</mark> It is an integral part of the [Copyright Act](https://indiankanoon.org/doc/1136195/) and therefore, it has to be given <mark>broad and liberal interpretation.</mark>

So public creativity is a real thing, fair dealing is a real defense for members of the public, Section 52 must be interpreted *broadly and liberally*. Essentially, users have "fair dealing" rights to all copyrighted work, specifically so that they can exercise their creativity, even if they don't have *copyright* itself. Copyright and Fair Dealing are *complementary*, i.e fair dealing does not imply that copyright was even violated in the first place.

It's starting to smell a lot like contracts aren't allowed to restrict Fair Dealing rights. 

*[Tekla vs. Survo Ghosh](https://indiankanoon.org/doc/164343914/)* Para. 17 states:

> I am also of the opinion that even if the holder of a copyright, <mark>though
> not entitled in law to impose any restrictions curtailing the fair use</mark> thereof or
> in the nature of <mark>curbing creativity</mark> (and which is <mark>against public policy</mark>), still
> <mark>contractually</mark> <mark>or otherwise</mark> <mark>imposes such restrictions</mark> or <mark>prohibits doing</mark> of
> <mark>anything permitted by [Section 52](https://indiankanoon.org/doc/1013176/)</mark> or any other provision of the [Copyright
> Act](https://indiankanoon.org/doc/1136195/) <mark>or any other law</mark>, the same would <mark>not bind anyone</mark> <mark>or be enforceable in
>  law</mark> and thereby not effect anyone. The legal action even if any taken by
> holder of copyright against any other person<mark> for violating the conditions
> illegally imposed by the holder of copyright</mark>, would thus <mark>fail</mark> and it cannot be
> said that there was any misuse.

So the answer leans towards **NO.** EULAs cannot take away your right to repair/hack/jailbreak/modify.

It also gets crazier. It means that whenever a given crime or protection in this act refers to "infringing any rights in this act", **it could go both ways.** It could **criminalise both copyright infringement and fair dealing rights infringement.** That means users might have the right to sue companies for violating their own fair dealing rights by punishing modding and jailbreaking.

##### "for the purpose for which it was supplied"

This clause is unclear and potentially restrictive on creativity and user freedom. 

As an example, let us say Google gives me the Google Chrome web browser. Google Chrome includes a feature called "Ad Topics", which effectively lets the browser spy on your browsing history to categorise what topics you are interested in, and then send them to data brokers/advertising companies so that they may target you with personalised web advertisements. This was the intended purpose for which the Ad Topics feature was supplied in Google Chrome, by its manufacturer Google. 

Assuming that you do not own your current copy of Google Chrome, because the EULA waived your ownership, are you not allowed to study and understand the functioning of the Ad Topics feature (ac) using a C++ debugger/decompiler in order to slowly but gradually remove its functionality, because that would be circumventing its' purpose?

##### Distribution and Collaboration

Jailbreaking tools are often developed not by one person, but a community of multiple people in collaboration. They may also broadcast their code, techniques, and knowledge to the public for fun/the public's benefit (e.g on web forums, social media, YouTube, and code-hosting platforms, and may promote these via. word of mouth or public seminars (e.g hacker conferences). Thus, it can be said that jailbreaking is in practice a **communal** practice and that both the acts as well as the products belong to the community as a whole, not only just every single involved individual as disconnected monads, nor just a private and selfish commercial entity that jealously guards its' secrets and techniques.

It is not clear from merely the statements in Section 52 whether the public at large has the rights to circulate and produce jailbreaking techniques, knowledge, and products among itself rather than it just being a right that is exercised by each individual participant. An individual right that does not recognise the ability to form and participate in communities would materially jeopardise the real world practices of hacking.

### Section 60: Remedy in the case of groundless threat of legal proceedings.

Where any person claiming to be the owner of copyright in any work, by circulars, advertisements or otherwise, <mark>threatens any other person with any legal proceedings or liability</mark> in respect of an alleged infringement of the copyright <mark>any person aggrieved thereby may</mark>, notwithstanding anything contained in section 34 of the Specific Relief Act, 1963 (47 of 1963), <mark>institute a declaratory suit that the alleged infringement to which the threats related was not in fact an infringement of any legal rights of the person making such threats</mark> and may in any such suit:

1. obtain an <mark>injunction against the continuance of such threats</mark>; and

2. <mark>recover such damages</mark>, if any, <mark>as he has sustained by reason of such threats</mark>:

Provided that <mark>this section does not apply</mark> if the person making such threats, with due diligence, <mark>commences and prosecutes an action</mark> for infringement of the copyright claimed by him.

#### Commentary

*Threatening* to sue a person for false copyright infringement is illegal, and you may enjoin them to stop, or recover any damages as such. (Could you recover the damage of e.g getting your Instagram account banned for "violating their ToS" by field testing and using a third-party client? That would be the final piece of the puzzle for protecting users from retaliation for exercising their fair-dealing rights, but it might jeopardise the platform's ability to legitimately defend against spam or data theft attempts by banning the perpetrators.)

However this does not prevent them from actually suing on the basis of (what may be a false) copyright infringement. That is then obviously the responsibility of the legal process to flesh out.

### Section 63: Offences of infringement of copyright or other rights conferred by this Act.

Any person who knowingly <mark>infringes or abets the infringement</mark> of:

1. The copyright in a work

2. <mark>any other right conferred by this Act</mark>, except the right conferred by section 53A,

shall be punishable with imprisonment for a term which shall not be less than six months but which may extend to three years and with fine which shall not be less than fifty thousand rupees but which may extend to two lakh rupees:

Provided that where the infringement has not been made for gain in the course of trade or business the court may, for adequate and special reasons to be mentioned in the judgment, impose a sentence of imprisonment for a term of less than six months or a fine of less than fifty thousand rupees.

#### Commentary

Infringing Section 52 rights is a crime. You are not allowed to technically interfere with the public's fair dealing rights. This could be a tool to actively defend fair dealing from corporate abuse, e.g account bans or technical lockouts.

### Section 65: Possession of plates for purpose of making infringing copies.

Any person who knowingly makes, or has in his possession, any plate for the purpose of making infringing copies of any work in which copyright subsists shall be punishable with imprisonment which may extend to two years and shall also be liable for fine.

#### Commnetary

A "plate for the purpose of making infringing copies" could be metaphorically interpreted to refer to jailbreak tools, cracks, modding tools, etc. Tools often have dual uses too; for example, a debugger may be used to break TPM, but this could be done either to pirate the application (infringement), or to program a new feature into it (not infringement). Thus,   the matter of intent of the tool is ultimately a matter of framing and bias.

### Section 65A: Protection of technological measures.

1. Any person who <mark>circumvents</mark> an <mark>effective technological measure</mark> <mark>applied for the purpose</mark> of <mark>protecting any of the rights conferred by this Act</mark>,<mark> with the intention of infringing such rights</mark>, shall be punishable with imprisonment which may extend to two years and shall also be liable to fine.

2. Nothing in sub-section (1) shall prevent any person from,—
   
   1. <mark>doing anything referred to therein</mark> <mark>for a purpose not expressly prohibited by this Act</mark>:
      
      1. Provided that <mark>any person facilitating circumvention by another person of a technological measure for such a purpose</mark> <mark>shall maintain a complete record of such other person</mark> including his name, address and all relevant particulars <mark>necessary to identify him and the purpose for which he has been facilitated</mark>; or
   
   2. <mark>doing anything</mark> <mark>necessary</mark> to <mark>conduct encryption research</mark> <mark>using a lawfully obtained encrypted copy</mark>; or
   
   3. <mark>conducting</mark> any <mark>lawful investigation</mark>; or
   
   4. <mark>doing anything necessary</mark> for the purpose of <mark>testing the security of a computer system or a computer network</mark> with the <mark>authorisation of its owner</mark>; or
   
   5. <mark>operator</mark>; or
   
   6. <mark>doing anything necessary</mark> to <mark>circumvent technological measures intended for identification or surveillance of a user</mark>; or
   
   7. <mark>taking measures necessary</mark> in the interest of <mark>national security.</mark>

#### Commentary

1. Circumvention *with the intention of committing copyright infringement* is a crime.

2. Does this mean you may *circumvent TPM with the intention of committing copyright infringement* if:
   
   1. It's for a purpose not prohibited by the Act
      
      1. If you get a friend, neighbour, or other person to do it for you, you must keep a record of them.
   
   2. doing anything to conduct encryption research using a lawfully *obtained* encrypted copy
      
      1. EMPRESS's CONDUCT IS LEGAL IN INDIA?
   
   3. A governmental/police investigation
   
   4. Pentesting a computer system or network with owner permission
   
   5. with operator permission
   
   6. Evading surveillance/tracking (e.g Adblocker, tracker blocker)
   
   7. For National Security

Part 1 lays it out; you can break any TPM if its' not for copyright infringement. Since Section 52 conduct isn't a copyright infringement, breaking TPM in order to perform is not a crime. Very very very free.

Part 2 is unclear to me. Does it just reiterate or give examples of conduct that was already legal under Part 1, or does it bizarrely in fact carve out even more exceptions of conduct done explicitly *for* the sole purpose of copyright infringement? I.e you can pirate if it's to save India? Huh?

This section explicitly refers to "rights conveyed by this act". Does that include Fair Dealing rights (Section 52)? If that's the case, could this be used to criminalise retaliation against interoperation? Hypothetically, consider a community that develops a sufficiently advanced Instagram client, which has some form of advanced anti-spoof detection measures, e.g user-agent strings, fingerprint/activity spoofing, etc. If Meta then applies patches to their network, in order to circumvent the spoofing done by the custom client community, with the intention of preventing the community from exercising their Section 52 rights, would this be a violation of Section 65A, but done by Meta? There are a lot of interesting ideas and novel inverted perspectives on copyright enforcement that could be developed from the idea of Section 52 exceptions being considered full-fledged statutory *rights*, as long as those enforcements refer to "rights under this act" (including both copyright and fair dealing rights) and not specifically only copyright.

### Section 65B: Protection of Rights Management Information.

Any person, who knowingly:

1. <mark>Removes</mark> or <mark>alters</mark> any <mark>rights management information</mark> without authority, or

2. <mark>distributes</mark>, <mark>imports for distribution</mark>, <mark>broadcasts or communicates to the public</mark>, without authority, <mark>copies of any work</mark>, or <mark>performance</mark> knowing that <mark>electronic rights management information</mark> has been <mark>removed or altered</mark> without authority, shall be punishable with imprisonment which may extend to two years and shall also be liable to fine:

Provided that if the rights management information has been tampered with in any work, the owner of copyright in such work may also avail of civil remedies provided under Chapter XII against the persons indulging in such acts.

#### Commentary

It is unclear from the clause what "rights management information" actually is. Some candidates come to mind:

1. The TPM program itself, either in source code or binary code form
   
   1. This would mean a legal fiction could be constructed by TPM users that in the course of circumventing TPM, "rights management information" was also neutered or removed (i.e modified or removed), which would be seen as illegal. 

2. The copyright notice, either plain or embedded

3. An embedded cryptographic private key/certificate, used to sign/permit some code. (E.g Nintendo Switch's boot keys)
   
   1. If, hypothetically, this was the answer, it may jeopardise some practices of repair that rely on extracting, spoofing, and re-using cryptographic keys embedded within derelict hardware or software, in order to rewrite them and modify them, or perhaps substitute manufacturer keys with custom owner/community keys (e.g supplying new certificates in order to get an old iOS device to connect to the modern app store.)

Until it is cleared up, this is a potential liability for aftermarket repairmen, and the repair/maintenance communities.

# A Layman's analysis of Jailbreaking wrt. The Information Technology Act, 2000

Tldr; *Is hacking an app somebody else made, running on your own computer, cybercrime? What about scraping, reverse engineering, and spoofing towards a network API to make an alternative client for it? What about systematically circumventing anti-scraping, anti-reverse-engineering, and spoof detection technology to avoid a technical ban for alternative client usage?*

It is unclear where jailbreaking or alternative client usage stand in the IT Act, as they are not defined anywhere. (The terminology is currently simple enough that it allows companies to claim that interoperation, TPM circumvention, and scraping are hacking. e.g Facebook shut down Barinsta, citing California's Computer Fraud and Abuse Act.)

It's already trite to mention how modern software no longer just works on its own, but architecturally requires a connection to a mothership server in order to do anything at all it's advertised for. Consumers recieve a mere dumb terminal, and the server is where the "interesting things" happen.

 One of the ways users have fought back against platform abuse is to make custom client applications that connect to the server, and act just like the normal app, while secretly removing or modifying any content according to their wishes, for example blocking ads or trackers. The server unwittingly works with the custom application and just sends away data. This worked for a long while, from the 1990s all the way until the mid 2010s, when centralised social media started wising up to the facts.

Today, software such as Instagram, WhatsApp, etc contain highly complex TPMs that have one purpose: detect if the user is using an unofficial client, and block them if they are, or permaban their accounts for deterrence. Detecting and deterring jailbreaking is itself one of the major areas of investment in user-facing technology, because given the opportunity the majority of users would *gladly* jailbreak and circumvent *the shit* out of all their tech to escape corporate abuse and spying *en masse*.

There are 3 angles used by companies to justify TPM:

1. Copyright violation (in India, this entire argument is false.)

2. Cybercrime
   
   1. Anti-scraping
   
   2. Fair use policies
   
   3. network ratelimits/anti spam protections

3. Publication or violation of a trade secret?

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

Here, a notion is developed that ownership of the program and data belongs only to the person owning or operating the computer resource, and that users may have several restrictions placed on them on what they can and cannot do. (Notably, server operators do not have the restriction placed on them that they mustn't discriminate against users on the basis of what client they're using.) The notion of user rights never enter the picture (i.e user access is suspicious by default, and may only be admitted according to the policy of the operator.)

Obtaining and utilising *unauthorised* access to a computer network is a crime. This is unambigously a legal threat to custom client users. The other clauses don't look friendly either. This requires more contemplation.

### Section 43A: Compensation for failure to protect data

Where a body corporate, possessing, dealing or handling any sensitive personal data or information in a computer resource which it owns, controls or operates, is <mark>negligent in implementing and maintaining reasonable security practices and procedures</mark> and thereby causes wrongful loss or wrongful gain to any person, such body corporate shall be liable to pay damages by way of compensation to the person so affected.

#### Commentary

A company could use this clause to argue that the act of engineering and utilising an (incidentally anti-consumer, anti-competitive, anti-creative) elaborate TPM system with opaque technical lockouts was necessary for maintaining security. The "security" excuse for everything.

## My commentary

I see a few broad issues:

1. It is unclear whether using a modified or custom client to access a computer resource (e.g a server, social media website's unofficial API, etc) is illegal, if it's not done in order to spam or DDoS the computer resource. The text of the statute fails to clarify any notion of user intention or user rights.

2. It is unclear whether the mere fact that an *unofficial* client is accessing a computer resource is enough to say that the other users of the resource are having their privacy violated by the unofficial client. If the user was using an *official* client, the computer resource would otherwise freely and publicly permit the access of user data (e.g users' posts, profile pictures, stories/statuses, direct messages, etc) as according to its' stated and promised function. When you run the Instagram website, it's not a privacy violation for others, but when you run a hypothetical vibecoded MacOS Desktop instagram+BlueSky combined client to download the photos your friend shared you, it's a privacy violation?

The over-collection of bot or client signals to determine whether a client is official or unofficial may itself be a severe violation of privacy and consumer rights, and overly ties the client and server together in an intentionally anticompetitive manner.

# Punishment and Deterrence for Jailbreaking

One of the most cruelest and effective methods to deter users from jailbreaking your social media app to block your creepy ads is to simply ban their accounts, IP addresses, content, and device fingerprints from your social media server. Users might stomach an ad-blocking client that breaks for a day while the client developers and the server administrators play their cat-and-mouse game, but they will absolutely be unable to handle getting their own accounts banned. Due to platform lock-in, users are often significantly attached to being able to contact their friends, family, colleagues, etc on the network, they literally cannot afford to lose their account or their life falls apart. So companies hold their entire digital presence hostage: if you try and break our unstated rules, we'll cut you off from everyone.

For example, I'm not even able to run WhatsApp on my phone, because it uses GrapheneOS, and my account once got banned for accidental spam years ago. To this day, the WhatsApp server (or client, not sure) somehow thinks that the combination of me running their app on an "unofficial" operating system, and using an account with a "prior history" of policy violation is enough to justify me being unable to access WhatsApp. So, I keep a dedicated old phone for running WhatsApp and lug it around with me everywhere, just to be able to communicate with people. All this in India, where practically all messaging is done through the WhatsApp network! It lets WhatsApp flex its' power to me; If I ever somehow piss WhatsApp off enough to get them to ban me permanently, I'd be completely cut off from my fellow college students, extended family, friends, and colleagues.

(You could say I should just drill down, decompile and jailbreak the app, keep up with the cat and mouse game forever. Or that maybe I should somehow get every single person I know to migrate all of their chats, groups, and organisation to Signal, Matrix, or XMPP. But those are exceedingly hard to do (I've tried, and it's hard because then everybody would have to do it to the next guy!), and somewhere along the way you've forgotten that it was never my responsibility to deal with, solve, or work around the problems that other people actively create. In talking personal responsibility, you've neglected to hold the exact offenders and tyrants responsible for their own crimes, which require all other people to adjust to them in the twisted version of personal responsibility, where people are expected to silently sit and accept whatever happens to them and passively adapt, rather than understand who's really at fault is upstream. This is not a natural disaster or a meteor strike where you technically do not possess the capability to solve the root cause; there is a named company run by living people with ultimately, technically, infinite agency, individually and collectively, who are the ones setting the conditions for this, and an enshittogenic policy environment that permits this kind of behaviour to begin with.)

What could be done about this? For starters, an analysis of user rights to their account access would be good. Perhaps it would rely on analysis of the DPDPA.
