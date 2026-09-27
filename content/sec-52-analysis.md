# A Layman's Analysis of Section 52(1)(aa)-(ad), Indian Copyright Act, 2012

Tldr; *Can software EULAs take away or legally restrict your precious Sec.52(1)(aa)-(ad) rights? Nobody knows*

This is my unqualified, highly WIP interpretation of Indian Copyright Law with a focus on software user rights. I highlight some terms in the clauses that I found interesting and concerningly poorly defined/tested, and raise a few nitpicky/conceptual doubts I've developed over the months and haven't found satisfactory answer to.

I've searched the internet for months for precedent regarding Sec.52(1)(aa)-(ad), but haven't found any. As far as I can tell, there is no clue yet how narrowly or broadly, pro-Big Tech or pro-user the courts would interpret it.

Here, I try to make a **copyright maximalist interpretation**, as a sort of "worst case" scenario of legal gaps that I think the Indian FOSS community, digital rights activists, consumer rights activists, or antimonopoly activists may face if they take up these things in court. If anybody has any info invalidating my interpretation, please reach out to me and I'd love to hear it and publish it here.

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

2. Stop copyright exhaustion on sale, (gratis) distribution, transfer (Section 14(a)(ii))? **YES (Engineering Analysis Centre of Excellence Ltd. vs CIT, 2021)**

### Section 52: ㅤㅤCertain acts not to be infringement of copyright

1. The following acts shall <mark>not constitute an infringement of copyright</mark>, namely:
   
   1. the <mark>making of copies</mark> or <mark>adaptation</mark> of a computer programme <mark>by the lawful possessor of a copy of such computer programme</mark>, <mark>from such copy</mark>
      
      1. <mark>in order to</mark> <mark>utilise</mark> the computer programme for the <mark>purpose for which it was supplied</mark>; or
      
      2. <mark>to make back-up copies</mark> <mark>purely</mark> as a <mark>temporary protection</mark> against <mark>loss, destruction or damage</mark> in order <mark>only to utilise</mark> the computer programme for <mark>the purpose for which it was supplied</mark>
   
   2. the <mark>doing of any act necessary</mark> to <mark>obtain information</mark> <mark>essential</mark> for <mark>operating interoperability</mark> of an <mark>independently created</mark> computer programmes[sic] <mark>with other programmer</mark>[sic] <mark>by a lawful possessor</mark> of <mark>a</mark> computer programme <mark>provided </mark>that <mark>such information</mark> is <mark>not otherwise readily available</mark>
   
   3. the <mark>observation</mark>, <mark>study</mark> or <mark>test</mark> <mark>of functioning</mark> of the computer programme <mark>in order to determine</mark> the <mark>ideas and principles</mark> which <mark>underline</mark> <mark>any elements of the programme</mark> <mark>while performing</mark> <mark>such acts</mark> <mark>necessary</mark> for the <mark>functions</mark> <mark>for which the computer programme was supplied</mark>
   
   4. the <mark>making of copies</mark> or <mark>adaptation</mark> of the computer programme <mark>from</mark> a <mark>personally</mark> <mark>legally obtained copy</mark> for <mark>non-commercial</mark> <mark>personal</mark> use

2. The provisions of sub-section (1) shall apply to the <mark>doing of any act</mark> <mark>in relation to the translation of a literary</mark>, dramatic or musical work <mark>or the adaptation of a literary</mark>, dramatic, musical or artistic work <mark>as they apply in relation to the work itself</mark>.

#### Commentary

My copyright maximalist interpretation of the above is thus. 

1. The following acts are not copyright infringements:
   
   1. Making verbatim, or modified copies of a program you lawfully possess (but do not have any part of copyright to), in order to
      
      1. Use that copy of the program. But only for the purpose that copy was supplied for, and not any novel, unintended, or contractually restricted usecase.
      
      2. Make backup copies only as a temporary protection against loss, destruction, or damage of that specific copy of the program. But to use those backups only for the purpose the original program was supplied for, not any novel, unintended, or contractually restricted usecase.
   
   2. Do only what is strictly necessary to any software, in order to obtain only the bare minimum information essential for operating the possibility of interoperability of any specifically independently created (i.e clean-room engineered) program with any other program. But only if that bare minimum required information is not already available, in any clear, confusing, or incomplete form, to the actor.
   
   3. The passive observation, study, or test (and explicitly not decompilation, debugging, clean-room-reproduction, or modification) of the readily apparent functioning or effects of the program, to understand how it works. But only if this study is done simultaneously while using the program for the purpose it was supplied for, and not for any novel, unintended, or contractually restricted usecase. (For example, you're not allowed to reverse engineer the weights or training process of a raw neural network program you have.)
   
   4. Making verbatim, or modified copies of a program you legally obtained (but do not have any part of copyright to) in a personal (and not commercial) capacity, and only for non-commercial (i.e recreational, academic use, not used in the course of employed/contracted commercial gain) and personal (i.e only for you, not for your friend, a small personally known audience, or the public at large)

# horrible horrible precedent

https://indiankanoon.org/docfragment/29401489/?formInput=decompile%20%20year%3A%202024

https://indiankanoon.org/doc/53468434/

https://indiankanoon.org/doc/115941294/

https://indiankanoon.org/search/?formInput=reverse+engineer
