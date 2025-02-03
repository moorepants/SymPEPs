SymPEP XXX — Establish a Governance Model
=========================================

**Author** Jason K. Moore, moorepants@gmail.com
**Status** Draft
**Type** Process
**Created** date created on, in yyyy-mm-dd format
**Resolution** url to discussion (required for Accepted | Rejected | Withdrawn)

## Abstract

The purpose of this SymPEP is to establish a new more democratic governance
model for the SymPy project. This model would superseed the model established
in 2011.

## Motivation and Scope

SymPy has grown to be a large project built from contributions of over 1200
developers with, likely, millions of users. Historically, the project has been
led with a "benevolent dictator" model with leadership starting with Ondrej
Certik and then passed to Aaron Meuerer. Out of the many scientific Python
projects, SymPy is one of the few with no formalized goverance model and one of
the few that has not formalized some form of democratic mechanisms for the
goverance. With no mechanism to make hard decisions, SymPy struggles to make
larger changes that can improve the software and/or community. Most other large
scientific Python software communities have decision making and leadership
transfer processes. When comparing SymPy to these communities, we are a bit
rougher around the edges and much less organized. To rememdy this, this SymPEP
proposes some new governance processes for SymPy, like regular in-person
goverance meetings, a board of core developers, democratic selection of
leaders, and limits of power.

## Usage and Impact

This section describes how users of SymPy will use features described in this
SymPEP. It should be comprised mainly of code examples that wouldn't be possible
without acceptance and implementation of this SymPEP, as well as the impact the
proposed changes would have on the ecosystem. This section should be written
from the perspective of the users of SymPy, and the benefits it will provide
them; and as such, it should include implementation details only if
necessary to explain the functionality.

Note that this section should *not* be treated as documentation of the
proposed functionality. Documentation should be included in the implementation
itself. The purpose of this section is to motivate why the change should be
made in the first place. See [SymPEP 1](SymPEP-0001) for more information.

## Backwards compatibility

### Current leadership model

Ondrej Certik started the project in 2006 and was the defacto "project leader".
He encouraged many people to join and help him develop the software, very much
leading by example. In January 2011, Ondrej officially [passed his leadership
role](https://groups.google.com/g/sympy/c/9FMoGT6gNcw/m/RFIP2UIIxJ8J) to Aaron
Meurer. Later in May 2011, Ondrej [declared what defined Aaron's role as
project
leader](https://groups.google.com/g/sympy/c/i-XD15syvqs/m/aeh2A2-YAKAJ):

Key things were:

- there is a "project owner" (Ondrej) and "project leader" (Aaron)
- project leader makes all code related decisions, owner cannot override leader
  on code decisions
- owner and leader define the "vision of SymPy"
- owner can override leader: 1) to replace the leader, 2) resolve conflict with
  leader and member

He also defined decision making:

- informal consensus (democracy) will be used to make decisions (+1/-1:
  referring to our pull request "voting" system at the time)
- if consensus cannot be reached project leader will make the decision
  ("benevolent dictator")
- project leader is responsible for balancing democratic and dictatorial
  decision making

It is important to note that there various things only some people have control
over:

- SymPy finances
- domain names
- github admin
- numfocus membership

As of May 2011, no new public declarations on the governance of SymPy have been
made other than maybe the introduction of SymPEPs in September 2023.

### Our decision making model in practice

Our current decision making process involves (mostly) public discussion on the
email list, live chat service, or the issue tracker. Most often, ideas are
proposed on the mailing list or as a patch via Github's pull request system and
become open for discussion. A tacit consensus decision making model then
follows, which basically means (for us):

- there should be at least one developer other than the proposer in support of
  the proposal (this relates to a general policy that every patch must be
  reviewed and approved by at least one another developer)
- if someone objects to the idea (i.e. a -1), it is up to the proposer to
  modify their idea until there are no objections
- absence of support or non-support assumes tacit approval from the community
  at large
- some reasonable time should be given for community members to weigh in and it
  up to the proposer to feel this out, i.e. bigger decisions need more time
- if no consensus can be reached, the project leader should make a decision

It has never been officially established who has the +1/-1 voting right, so
theorectically anyone can do so, even if they are not part of the SymPy
community. SymPy also unofficially seems to support a meritocracy, i.e. the
more you do the more decision making power you gain. If you do "enough" and ask
for push access, you can be granted it by the project leader. We sometimes
refer to the group of contributors who have push access to the Github
repository as the "core developers".

At some point, the +1/-1 style voting on the patch discussion has decreased,
with some developers possibly using the GIthub "thumb's up/down" emoji in the
same way.

The existing decision making model works well for small to medium changes to
the code base, but often feels lacking for large proposals to the code or to
the community. Many scientific Python communities followed the Python language
community in using Python Enhancement Proposals to address this and SymPy
adopted this with the merger of SymPEP 001 in September 2023, but there has
been little to no use of the system since then.

## Detailed description

This SymPEP proposes:

- retain tacit consensus for small to medium changes
- SymPEPs for large changes
- move to a board with formalized voting
- introduce quartely video conferences
- public finances

## Related Work

This section should list relevant and/or similar technologies, possibly in other
libraries. It does not need to be comprehensive, just list the major examples of
prior and relevant art.

## Implementation

This section lists the major steps required to implement the SymPEP.  Where
possible, it should be noted where one step is dependent on another, and which
steps may be optionally omitted.  Where it makes sense, each step should
include a link to related pull requests as the implementation progresses.

Any pull requests or development branches containing work on this SymPEP should
be linked to from here.  (A SymPEP does not need to be implemented in a single
pull request if it makes sense to implement it in discrete phases).

## Alternatives

If there were any alternative solutions to solving the same problem, they should
be discussed here, along with a justification for the chosen approach.

## Discussion

This section may just be a bullet list including links to any discussions
regarding the SymPEP. All issues, pull requests, discussions, and mailing list
threads relating to a SymPEP should be listed and hyperlinked here.

## References

Any references should be listed here. Note this does not include links to
discussions about the SymPEP, which are listed in the previous section. For
online resources, freely accessible and stable online resources such as
Wikipedia, Wolfram MathWorld, and the NIST Digital Library of Mathematical
Functions (DLMF), which are unlikely to suffer from hyperlink rot, should be
preferred. Non-online references such as textbook or literature references may
also be used here.

## Copyright

Each SymPEP must be explicitly labeled as placed in the public domain, using
the below sentence (the below sentence also applies to this template).

This document has been placed in the public domain.

## Extra Notes About SymPEPs

NOTE: This section is not part of the template. It should not be included in
any SymPEPs. It is a list of notes of things that apply to all parts of the
above template.

Some extra notes about writing a SymPEP:

- All SymPEPs live in the [SymPEPs
  repository](https://github.com/sympy/SymPEPs/) on GitHub. All proposed
  SymPEPs should be made as pull requests to that repo (see [SymPEP
  1](SymPEP-0001)).
- The number corresponding to a SymPEP will be assigned when it is first
  proposed to the community. You may use `XXXX` as a placeholder number until
  this is done.
- The file for a SymPEPs should be named `SymPEP-XXXX.md` where `XXXX` is a
  four digit number, preceded with leading 0s. It should be placed at the root
  of the [SymPEPs repository](https://github.com/sympy/SymPEPs/).
- All SymPEP documents should be written in Markdown, following this template.
  The Markdown should be compatible with GitHub Flavored Markdown, so that the
  SymPEPs are viewable on GitHub. This means that Markdown features
  not supported by GitHub, such as footnotes, should be avoided.
- Any references to other SymPEPs should be written as internal links, e.g.,
  [SymPEP 1](SymPEP-0001).
- Images or diagrams may be included in the SymPEP if they improve the
  understanding of the discussion. Code examples should always be included as
  plain text. Any image or diagram should be accompanied by corresponding text
  describing what is in it. Images should be stored in an `images` directory
  at the root of the SymPEPs repository. Images should be titled like
  `XXXX-image-name.svg` where `XXXX` is the four digit number of the SymPEP
  and `image-name` is the name of the image. For example,
  `images/0001-process-diagram.svg`. Vector images are preferred when
  possible. Note that images should only be included when they significantly
  improve the discussion in the SymPEP. The vast majority of SymPEPs should
  not include images.
- All sections in the template are not necessarily required, but are
  encouraged. Including them will help you succeed with your proposal.
