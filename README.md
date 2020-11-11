# RPLv2

Todo List
---------

* Alvaro: Note that "SHOULD respond with a DAO-ACK" leaves the door open to not doing it. Unfortunately rfc6550 didn't explicitly mention what may be the reasons to not send a DAO-ACK (or not using MUST instead). TODO: change to MUST.

* Benjamin: about  draft-ietf-roll-turnon-rfc8138-17 

I will say a bit more inline, but want to note upfront that my primary unease here is that we seem to be assigning some (partial) semantics to MOP value 7 here (even though we do not specify full semantics for MOP value 7):

         For a MOP value of 7, [RFC8138] MUST be used on Links where 6LoWPAN Header Compression [RFC6282] applies and MUST NOT be used otherwise.

yet there is no "trail of breadcrumbs" for someone to follow from "I want to implement MOP 7" and end up at the sentence I quoted above.  A formal Update to 6550 would provide such a trail, as would being listed as a reference in the IANA registry for MOP value 7.  My current understanding is that the only thing we have right now is "repeat this requirement in whatever document ends up providing a full specification for MOP value 7", and I don't think that relying on the IETF's collective memory is a great way to enforce such a requirement -- we can and have in the past slipped up and published RFCs that are inconsistent with requirements imposed by previous ones.

"
