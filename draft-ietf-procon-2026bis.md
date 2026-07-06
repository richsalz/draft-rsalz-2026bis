---
title: "The Internet Standards Process"
abbrev: "process"
docname: draft-ietf-procon-2026bis-latest
submissiontype: IETF
category: bcp
ipr: trust200902
area: General
workgroup: procon
keyword: process
stand_alone: yes
smart_quotes: no
obsoletes: 2026, 5657, 6410, 7100, 7127, 8789, 9282
updates: 7475
pi: [toc, sortrefs, symrefs]

author:
 -
    ins: R. Salz
    name: Rich Salz
    organization: Akamai Technologies
    email: rsalz@akamai.com
 -
    ins: S. Bradner
    name: Scott Bradner
    organization: Harvard University (retired)
    email: sob@sobco.com

venue:
 repo: https://github.com/ietf-wg-procon/2026bis

normative:

informative:
    2418bis: I-D.draft-ietf-procon-2418bis
    ADSPONSOR:
      title: Guidance on Area Director Sponsoring of Documents
      target: https://datatracker.ietf.org/doc/statement-iesg-guidance-on-area-director-sponsoring-of-documents-20070320/
      date: "March 20, 2007"
    RFCXML:
      title: RFCXML overview and background
      target: https://authors.ietf.org/rfcxml-overview
    RFCPAGE:
      title: About RFCs
      target: https://www.ietf.org/process/rfcs/
    REQPAGE:
      title: Required Content
      target: https://authors.ietf.org/en/required-content
      date: "June, 2025"
    IDPAGE:
      title: Internet-Drafts
      target: https://www.ietf.org/participate/ids/
    UNICODE:
      title: The Unicode Standard
      author:
      - organization: "Unicode Technical Committee"
      date: "September 9, 2025"
      ann: "Unicode 17.0.0"

--- abstract

This memo documents the process used by the Internet community for
the standardization of protocols and procedures. It defines the
stages in the standardization process, the requirements for moving a
document between stages, and the types of documents used during this
process. It also addresses the intellectual property rights and
copyright issues associated with the standards process.

This document obsoletes RFC 2026, RFC 5657, RFC 6410, RFC 7100, RFC 7127,
RFC 8789, and
RFC 9282.  It also includes the changes from
RFC 7475.
If this document and {{2418bis}} are published as RFCs, then
taken together the two of them make RFC 7475 obsolete.

--- middle

# Introduction

This memo documents the process currently used by the Internet
community for the standardization of protocols and procedures. The
Internet Standards process is organized and managed by the IETF,
an entity of the Internet Society (ISOC); see {{!RFC8712}}.

The Internet, a loosely-organized international collaboration of
autonomous, interconnected networks, supports host-to-host
communication through voluntary adherence to open protocols and
procedures defined by Internet Standards. There are also many
isolated interconnected networks, which are not connected to the
global Internet but use the Internet Standards.

The Internet Standards Process described in this document is
concerned with all protocols, procedures, and conventions that are
used in or by the Internet, whether or not they are part of the
TCP/IP protocol suite. In the case of protocols developed and/or
standardized by non-Internet organizations, however, the Internet
Standards Process normally applies to the application of the protocol
or procedure in the Internet context, not to the specification of the
protocol itself.

In general, an Internet Standard is a specification that is stable
and well-understood, is technically competent, has multiple,
independent, and interoperable implementations with substantial
operational experience, enjoys significant public support, and is
recognizably useful in some or all parts of the Internet.

## Terminology

Readers are expected to be familiar with the various entities
involved in the Internet Standards Process, as described in {{!RFC9281}}.

# Creating an Internet Standard

A specification undergoes a period of development
and several iterations of review by the Internet community and
revision based upon experience, is then adopted as a Standard by the
appropriate body (see below), and is published. In practice, the
process is more complicated, due to (1) the difficulty of creating
specifications of high technical quality; (2) the need to consider
the interests of all of the affected parties; (3) the importance of
establishing widespread community consensus; and (4) the difficulty
of evaluating the utility of a particular specification for the
Internet community.

The process described here only applies to the IETF RFC stream.  See
{{?RFC4844}} for the definition of the streams and {{?RFC5742}} for a
description of the IESG responsibilities related to those streams.

The goals of the Internet Standards Process are:

- Technical excellence;

- Prior implementation and testing;

- Clear, concise, and easily-understood documentation;

- Openness and fairness; and

- Timeliness

The procedures described in this document are designed to be fair,
open, and objective; to reflect existing (proven) practice; and to
be flexible.

- These procedures are intended to provide a fair, open, and
objective basis for developing, evaluating, and adopting Internet
Standards. They provide ample opportunity for participation and
comment by all interested parties. At each stage of the
standardization process, a specification is repeatedly discussed
and its merits debated in open meetings, public electronic
mail lists, and/or other electronic fora, and it is made available
for review via world-wide on-line directories.

- These procedures are explicitly aimed at recognizing and adopting
generally-accepted practices. Thus, a candidate specification
must be implemented and tested for correct operation and
interoperability by multiple independent parties and utilized in
increasingly demanding environments, before it can be adopted as
an Internet Standard.

- These procedures provide a great deal of flexibility to adapt to
the wide variety of circumstances that occur in the
standardization process. Experience has shown this flexibility to
be vital in achieving the goals listed above.

The goal of technical competence, the requirement for prior
implementation and testing, and the need to allow all interested
parties to comment all require significant time and effort. On the
other hand, today's rapid development of networking technology
demands timely development of standards. The Internet Standards
Process is intended to balance these conflicting goals. The process
is believed to be as short and simple as possible without sacrificing
technical excellence, thorough testing before adoption of a standard,
or openness and fairness.

From its inception, the Internet has been, and is expected to remain,
an evolving system whose participants regularly factor new
requirements and technology into its design and implementation. Users
of the Internet and providers of the equipment, software, and
services that support it should anticipate and embrace this evolution
as a major tenet of Internet philosophy.

The procedures described in this document are the result of a number
of years of evolution, driven both by the needs of the growing and
increasingly diverse Internet community, and by experience.

## Intellectual Property Requirements {#ipr-requirements}

All documents used in the Internet Standards Process must meet the
conditions specified in {{!BCP78}} and {{!BCP79}}.

# Organization of This Document

{{sec2}} describes the publications and archives of the Internet
Standards Process. {{sec3}} describes the types of Internet
standard specifications. {{sec4}} describes the Internet standards
specifications track. {{sec5}} describes Best Current Practice
RFCs. {{sec6}} describes the process and rules for Internet
standardization. {{sec7}} specifies the way in which externally-
sponsored specifications and practices, developed and controlled by
other standards bodies or by others, are handled within the Internet
Standards Process. {{sec8}} describes the requirements for notices
and record keeping, and {{sec9}} defines a variance process to allow
one-time exceptions to some of the requirements in this document.

# Documents related to Internet Standards {#sec2}

## Requests for Comments (RFCs)

Each distinct version of an Internet Standards specification
is published as an RFC on the IETF stream.
RFCs can be obtained from a number of
Internet hosts using standard Internet applications such as the WWW.

RFCs cover a wide range of
topics in addition to Internet Standards, from early discussion of
new research concepts to status memos about the Internet.
For information about RFC publication, see {{?RFC9920}}.

The style guide for writing an RFC is {{!RFC7322}}.
The default input format is {{RFCXML}},
RFCs are available in multiple formats as described in {{RFCPAGE}}.

Some RFCs document an "Internet Standard." These RFCs form the "STD"
subseries of the RFC series {{?RFC1311}}. When a specification has been
adopted as an Internet Standard, it is given the additional label
"STD xxx" (see {{sec413}}).

Some RFCs standardize the results of community deliberations about
statements of principle or conclusions about what is the best way to
perform some operations or IETF processes. These RFCs form
Best Current Practice (BCP) subseries. When a specification has
been adopted as a BCP, it is given the
additional label "BCP xxx" (see {{sec5}}).

Each entry in the STD or BCP subseries may have more than one RFC.

Not all specifications of protocols or services for the Internet
should or will become Internet Standards or BCPs. Such non-standards
track specifications are not subject to the rules for Internet
standardization. Non-standards track specifications may be published
as "Experimental" or "Informational" RFCs; see {{sec42}}.

In addition, not all RFCs are standards track documents, and not all
standards track documents reach the level of Internet Standard. In the same
way, not all RFCs which describe current practices have been given the review
and approval to become BCPs. See {{!RFC1796}} for further information.

The full list of all RFCs, including the subseries, and lists organized
by status, can be found at
[https://www.rfc-editor.org](https://www.rfc-editor.org).

## Internet-Drafts {#sec22}

During the development of a specification, draft versions of the
document are made available to the public for review and comment by
placing them in the Internet-Drafts collection {{IDPAGE}}.  This
makes an evolving working document readily available to a wide audience,
facilitating the process of review and revision.

A Internet-Draft that has been not been changed for more than six months
will be marked as Expired and may be removed from some views of the
collection.  At any time, an Internet-Draft may be replaced by a more
recent version of the same specification, restarting the six-month
timeout period.

The format of an Internet-Draft is mostly the same as for an RFC
as described in {{?RFC7322, Section 4}}.
Full details, including the naming conventions and required contents, can be
found at {{REQPAGE}}.  Of particular importance is the legal boilerplate
and copyright as described in the "Copyright Notice" section of that page.

Internet-Drafts have no formal status, and are subject to change or
removal at any time.  They are working documents and have no official
standards status whatsoever. They may, eventually, turn into a
standards-track document or they may sink from sight. An Internet-Draft
is not a means of "publishing" a specification; specifications are
published through the RFC mechanism described in the previous section.

It is acceptable to reference an Internet-Draft that may reasonably be
expected to be published as an RFC using the phrase "Work in Progress".
This may also be done in a standards track document itself as long as
the specification in which the reference is made would stand as a
complete and understandable document with or without the reference to
the "Work in Progress".

# Internet Standard Specifications {#sec3}

Specifications subject to the Internet Standards Process fall into
one of two categories: Technical Specification (TS) and
Applicability Statement (AS).

## Technical Specification

A Technical Specification is any description of a protocol, service,
procedure, convention, or format. It may completely describe all of
the relevant aspects of its subject, or it may leave one or more
parameters or options unspecified. A TS may be completely self-
contained, or it may incorporate material from other specifications
by reference to other documents (which might or might not be Internet
Standards).

A TS shall include a statement of its scope and the general intent
for its use (domain of applicability). Thus, a TS that is inherently
specific to a particular context shall contain a statement to that
effect. However, a TS does not specify requirements for its use
within the Internet; these requirements, which depend on the
particular context in which the TS is incorporated by different
system configurations, are defined by an Applicability Statement.

## Applicability Statement {#sec32}

An Applicability Statement specifies how, and under what
circumstances, one or more TSs may be applied to support a particular
Internet capability. An AS may specify uses for TSs that are not
Internet Standards, as discussed in {{sec7}}.

An AS identifies the relevant TSs and the specific way in which they
are to be combined, and may also specify particular values or ranges
of TS parameters or subfunctions of a TS protocol that must be
implemented. An AS also specifies the circumstances in which the use
of a particular TS is required, recommended, or elective (see {{sec33}}).

An AS may describe particular methods of using a TS in a restricted
"domain of applicability", such as Internet routers, terminal
servers, Internet systems that interface to Ethernets, or datagram-
based database servers.

The broadest type of AS is a comprehensive conformance specification,
commonly called a "requirements document", for a particular class of
Internet systems, such as Internet routers or Internet hosts.

An AS may not have a higher maturity level in the standards track
than any standards-track TS on which the AS relies (see {{sec41}}).

## Requirement Levels {#sec33}

An AS shall apply one of the following "requirement levels" to each
of the TSs to which it refers:

- Required: Implementation of the referenced TS, as specified by
the AS, is required to achieve minimal conformance. For example,
IP and ICMP must be implemented
by all Internet systems using the
TCP/IP Protocol Suite.

- Recommended: Implementation of the referenced TS is not
required for minimal conformance, but experience and/or generally
accepted technical wisdom suggest its desirability in the domain
of applicability of the AS. Vendors are strongly encouraged to
include the functions, features, and protocols of Recommended TSs
in their products, and should omit them only if the omission is
justified by some special circumstance. For example, the TELNET
protocol should be implemented by all systems that would benefit
from remote access.

- Elective or Optional: Implementation of the referenced TS is not
mandatory
within the domain of applicability of the AS; that is, the AS
creates no explicit necessity to apply the TS. However, a
particular vendor may decide to implement it, or a particular user
may decide that it is a necessity in a specific environment.

As noted in {{sec41}}, there are TSs that are not in the
standards track or that have been retired from the standards
track, and are therefore not required, recommended, or elective.
Two additional "requirement level" designations are available for
these TSs:

- Limited Use: The TS is considered to be appropriate for use
only in limited or unique circumstances. For example, the usage
of a protocol with the "Experimental" designation should generally
be limited to those actively involved with the experiment.

- Not Recommended: A TS that is considered to be inappropriate
for general use is labeled "Not Recommended". This may be because
of its limited functionality, specialized nature, or historic
status.

Although TSs and ASs are conceptually separate, in practice a
standards-track document may combine an AS and one or more related
TSs. For example, Technical Specifications that are developed
specifically and exclusively for some particular domain of
applicability, e.g., for mail server hosts, often contain within a
single specification all of the relevant AS and TS information. In
such cases, no useful purpose would be served by deliberately
distributing the information among several documents just to preserve
the formal AS/TS distinction. However, a TS that is likely to apply
to more than one domain of applicability should be developed in a
modular fashion, to facilitate its incorporation by multiple ASs.

# The Internet Standards Track {#sec4}

Specifications that are intended to become Internet Standards evolve
through a set of maturity levels known as the "standards track".
These maturity levels -- "Proposed Standard" and "Internet Standard" --
are defined and discussed in {{sec41}}. The way in
which specifications move along the standards track is described in
{{sec6}}.

There used to be a status that came between Proposed Standard and Internet
Standard called "Draft Standard." As of the writing of this document, there
still exist some RFCs at that status. Documents at Draft Standard may be
advanced to Internet Standard, either via the procedure described in {{sec6}}
(if they meet the requirements of {{propstd}}) or with the consent of the
IESG. The IESG may also decide to remove the Draft Standard status from a
document and mark it as either Historic or Proposed Standard.

Even after a specification has been adopted as an Internet Standard,
further evolution often occurs based on experience and the
recognition of new requirements. The nomenclature and procedures of
Internet standardization provide for the replacement of old Internet
Standards with new ones, and the assignment of descriptive labels to
indicate the status of "retired" Internet Standards. A set of
maturity levels is defined in {{sec42}} to cover these and other
specifications that are not considered to be on the standards track.

Standards track specifications normally must not depend on either
other standards track specifications which are at a lower maturity
level or on non standards track specifications other than referenced
specifications from other standards bodies (see {{!BCP97}} and {{sec7}}).

## Standards Track Maturity Levels {#sec41}

Internet specifications go through stages of development, testing,
and acceptance. Within the Internet Standards Process, these stages
are formally labeled "maturity levels".

This section describes the maturity levels and the expected
characteristics of specifications at each level.

A "standards action" -- entering a particular specification into,
advancing it within, or removing it from, the standards track -- must
be approved by the IESG.

### Proposed Standard {#propstd}

The entry-level maturity for the standards track is "Proposed
Standard."  A specific action by the IESG is required to move a
specification onto the standards track at the "Proposed Standard"
level.

A Proposed Standard specification is stable, has resolved known
design choices, has received significant community review, and
appears to enjoy enough community interest to be considered valuable.

Usually, neither implementation nor operational experience is
required for the designation of a specification as a Proposed
Standard.  However, such experience is highly desirable and will
usually represent a strong argument in favor of a Proposed Standard
designation.

The IESG may require implementation and/or operational experience
prior to granting Proposed Standard status to a specification that
materially affects the core Internet protocols or that specifies
behavior that may have significant operational impact on the
Internet.

A Proposed Standard will have no known technical omissions with
respect to the requirements placed upon it.  Proposed Standards are
of such quality that implementations can be deployed in the Internet.
However, as with all technical specifications, Proposed Standards may
be revised if problems are found or better solutions are identified,
when experiences with deploying implementations of such technologies
at scale is gathered.

Notwithstanding the previous paragraph, the IETF may occasionally
choose to publish as Proposed Standard a
document that contains areas of known limitations or challenges.  In
such cases, any known issues with the document will be clearly and
prominently communicated in the document, for example, in the
abstract, the introduction, or a separate section or statement.


### Internet Standard {#sec413}

A specification for which significant implementation and successful
operational experience has been obtained may be elevated to the
Internet Standard level. An Internet Standard
is characterized by a high degree of
technical maturity and by a generally held belief that the specified
protocol or service provides significant benefit to the Internet
community.

A specification that reaches the status of Internet Standard is
assigned a number in the STD subseries.

## Non-Standards Track Maturity Levels {#sec42}

Not every specification is on the standards track. A specification
may not be intended to be an Internet Standard, or it may be intended
for eventual standardization but not yet ready to enter the standards
track. A specification may have been superseded by a more recent
Internet Standard, or have otherwise fallen into disuse or disfavor.

Specifications that are not on the standards track are labeled with
one of three "off-track" maturity levels: "Experimental,"
"Informational," or "Historic." The documents bearing these labels
are not Internet Standards in any sense, but they must also be
approved by the IESG.

### Experimental

The "Experimental" designation typically denotes a specification that
is part of some research or development effort. Such a specification
is published for the general information of the Internet technical
community and as an archival record of the work.

### Informational

An "Informational" specification is published for the general
information of the Internet community. The Informational
designation is intended to provide for the timely publication of a
very broad range of responsible informational documents from many
sources.

### Procedures for Experimental and Informational RFCs {#sec423}

Documents with the Experimental or Informational maturity level
may be published using the process and workflow described here.
Documents proposed for Experimental and Informational RFCs by IETF
Working Groups {{2418bis}} go through IESG review.
The review is initiated using
the process described in {{sec611}}.

The final assignment of maturity level, as with Internet Standards
Track Documents,
is determined by the IESG.

### Historic

A specification that has been superseded by a more recent
specification or is for any other reason considered to be obsolete is
assigned to the "Historic" level. (Purists have suggested that the
word should be "Historical"; however, at this point the use of
"Historic" is historical.)

# Best Current Practice (BCP) RFCs {#sec5}

The BCP subseries of the RFC series is designed to be a way to
standardize practices and the results of community deliberations. A
BCP document is subject to the same basic set of procedures as
standards track documents and thus is a vehicle by which the IETF
community can define and ratify the community's best current thinking
on a statement of principle or on what is believed to be the best way
to perform some operations.

Historically Internet Standards have generally been concerned with
the technical specifications for hardware and software required for
computer communication across interconnected networks. However,
since the Internet itself is composed of networks operated by a great
variety of organizations, with diverse goals and rules, good user
service requires that the operators and administrators of the
Internet follow some common guidelines for policies and operations.
While these guidelines are generally different in scope and style
from protocol standards, their establishment needs a similar process
for consensus building.

Finally, the BCP subseries may be used to document the operation of the
IETF itself. For example, this document defines the IETF Standards
Process and is published as a BCP.

## BCP Review Process {#sec51}

Unlike standards-track documents, the mechanisms described in BCPs
are not well suited to the phased roll-in nature of the two-stage
standards track and instead generally only make sense for full and
immediate instantiation.

The BCP process is similar to that for proposed standards. The BCP
is submitted to the IESG for review (see {{sec611}}), and the
existing review process applies, including a Last-Call on the IETF
Announce mailing list. However, once the IESG has approved the
document, the process ends and the document is published. The
resulting document is viewed as having the technical approval of the
IETF.

Specifically, a document to be considered for the status of BCP must
undergo the procedures outlined in {{sec6}}, and {{sec64}} of this
document. The BCP process may be appealed according to the procedures
in {{sec65}}.

Because BCPs are meant to express community consensus but are arrived
at more quickly than standards, BCPs require particular care.
Specifically, BCPs should not be viewed simply as stronger
Informational RFCs, but rather should be viewed as documents suitable
for a content different from Informational RFCs.

A specification, or group of specifications, that has, or have been
approved as a BCP is assigned a number in the BCP subseries.

# Standards Actions {#sec6}

A "standards action" -- entering a particular specification into,
advancing it within, or removing it from, the standards track -- must
be approved by the IESG.

The mechanics of the Internet Standards Process involve decisions of
the IESG concerning the elevation of a specification onto the
standards track or the movement of a standards-track specification
from one maturity level to another. Although a number of reasonably
objective criteria (described below and in {{sec4}}) are available
to guide the IESG in making a decision to move a specification onto,
along, or off the standards track, there is no algorithmic guarantee
of elevation to or progression along the standards track for any
specification. The experienced collective judgment of the IESG
concerning the technical quality of a specification proposed for
elevation to or advancement in the standards track is an essential
component of the decision-making process.

## Initiation of Action {#sec611}

A specification that is intended to enter or advance in the Internet
standards track shall first be posted as an Internet-Draft (see
{{sec22}}) unless it has not changed since publication as an RFC.
It shall remain as an Internet-Draft for a period of time, not less
than two weeks, that permits useful community review, after which a
recommendation for action may be initiated.

A standards action is initiated by a recommendation by the IETF
Working group responsible for a specification to its Area Director,
copied to the IETF Secretariat or, in the case of a specification not
associated with a Working Group, a recommendation by an individual to
the IESG.

For classification as an Internet Standard, the request for reclassification
must include an explanation of how the following criteria have
been met:

1. There are at least two independent interoperating implementations
with widespread deployment and successful operational experience.
Although not required by the Internet Standards Process, {{?RFC5657}}
can be helpful to conduct interoperability testing.

2. There are no errata against the specification that would cause a
new implementation to fail to interoperate with deployed ones.

3. There are no unused features in the specification that greatly
increase implementation complexity.

4. If the technology required to implement the specification
requires patented or otherwise controlled technology, then the
set of implementations must demonstrate at least two independent,
separate and successful uses of the licensing process.

## IESG Review and Approval {#sec612}

The IESG shall determine whether or not a specification submitted to
it according to {{sec611}} satisfies the applicable criteria for
the recommended action (see {{sec41}} and {{sec42}}), and shall in
addition determine whether or not the technical quality and clarity
of the specification is consistent with that expected for the
maturity level to which the specification is recommended.

In order to obtain all of the information necessary to make these
determinations, particularly when the specification is considered by
the IESG to be extremely important in terms of its potential impact
on the Internet or on the suite of Internet protocols, the IESG may,
at its discretion, commission an independent technical review of the
specification.

The IESG will send notice to the IETF of the pending IESG
consideration of the document(s) to permit a final review by the
general Internet community. This "Last-Call" notification shall be
via electronic mail to the IETF Announce mailing list. Comments on a
Last-Call shall be accepted from anyone, and should be sent as
directed in the Last-Call announcement.

Except as described below,
the Last-Call period shall be no shorter than two weeks except in
those cases where the proposed standards action was not initiated by
an IETF Working Group, such as when an AD sponsors a draft {{ADSPONSOR}},
in which case the Last-Call period shall be no
shorter than four weeks. If the IESG believes that the community
interest would be served by allowing more time for comment, it may
decide on a longer Last-Call period or to explicitly lengthen a
current Last-Call period.

For an Internet Standard, the IESG will perform a review and
consideration of any errata that have been filed.
If they do not believe any of these should hold up the
advancement, then
the IESG, in an IETF-wide Last Call of at least four weeks,
informs the community of their intent to advance a document
from Proposed Standard to Internet Standard.

If there is consensus for
reclassification, the RFC will be reclassified with or
without publication of a new RFC.

In a timely fashion after the expiration of the Last-Call period, the
IESG shall make its final determination of whether or not to approve
the standards action, and shall notify the IETF of its decision via
electronic mail to the IETF Announce mailing list.

The IESG is not bound by the action recommended when the
specification was submitted. For example, the IESG may decide to
consider the specification for publication in a different maturity level
than that requested. If the IESG determines this before the Last-
Call is issued then the Last-Call should reflect the IESG's view.
The IESG could also decide to change the publication maturity level based
on the response to a Last-Call. If this decision would result in a
specification being published at a "higher" level than the original
Last-Call was for, a new Last-Call should be issued indicating the
IESG recommendation. In addition, in case of significant controvery
in response to the Last-Call, The IESG may decide to refer the document back to
the Working Group, the authors, or hold the document for the creation
of a new Working Group.

## Publication

In no event shall a document be published on the IETF Stream
without IETF consensus.

If a standards action is approved, notification is sent to the RFC
Editor and copied to the IETF with instructions to publish the
specification as an RFC. The specification shall at that point be
removed from the Internet-Drafts directory.

## Advancing in the Standards Track

The procedure described in {{sec6}} is followed for each action
that attends the advancement of a specification along the standards
track.

A specification shall remain at the Proposed Standard level for at
least six months.
This minimum period is intended to ensure adequate opportunity for
community review without severely impacting timeliness. The
interval shall be measured from the date of publication of the
corresponding RFC(s), or, if the action does not result in RFC
publication, the date of the announcement of the IESG approval of the
action.

A specification may be (indeed, is likely to be) revised as it
advances through the standards track. At each stage, the IESG shall
determine the scope and significance of the revision to the
specification, and, if necessary and appropriate, modify the
recommended action. Minor revisions are expected, but a significant
revision may require that the specification accumulate more
experience at its current maturity level before progressing. Finally,
if the specification has been changed very significantly, the IESG
may recommend that the revision be treated as a new document, re-
entering the standards track at the beginning.

Change of status shall result in republication of the specification
as an RFC, except in the rare case that there have been no changes at
all in the specification since the last publication. Generally,
desired changes will be "batched" for incorporation at the next level
in the standards track. However, deferral of changes to the next
standards action on the specification will not always be possible or
desirable; for example, an important typographical error, or a
technical error that does not represent a change in overall function
of the specification, may need to be corrected immediately. In such
cases, the IESG or RPC may be asked to republish the RFC (with
a new number) with corrections, and this will not reset the minimum
time-at-level clock.

## Revising a Standard {#sec63}

A new version of an established Internet Standard must progress
through the full Internet standardization process as if it were a
completely new specification. Once the new version has reached the
Standard level, it will usually replace the previous version, which
will be moved to Historic status. However, in some cases both
versions may remain as Internet Standards to honor the requirements
of an installed base. In this situation, the relationship between
the previous and the new versions must be explicitly stated in the
text of the new version or in another appropriate document (e.g., an
Applicability Statement; see {{sec32}}).

## Retiring a Standard {#sec64}

As the technology changes and matures, it is possible for a new
Standard specification to be so clearly superior technically that one
or more existing standards track specifications for the same function
should be retired. In this case, or when it is felt for some other
reason that an existing standards track specification should be
retired, the IESG shall approve a change of status of the old
specification(s) to Historic. This recommendation shall be issued
with the same Last-Call and notification procedures used for any
other standards action. A request to retire an existing standard can
originate from a Working Group, an Area Director or some other
interested party.

## Conflict Resolution and Appeals {#sec65}

Disputes are possible at various stages during the IETF process. As
much as possible the process is designed so that compromises can be
made, and genuine consensus achieved, however there are times when
even the most reasonable and knowledgeable people are unable to
agree. To achieve the goals of openness and fairness, such conflicts
must be resolved by a process of open review and discussion. This
section specifies the procedures that shall be followed to deal with
Internet Standards Process issues that cannot be resolved through the normal
processes whereby IETF Working Groups and other Internet Standards
Process participants ordinarily reach consensus.

### Working Group Disputes

An individual (whether a participant in the relevant Working Group or
not) may disagree with a Working Group recommendation based on his or
her belief that either (a) his or her own views have not been
adequately considered by the Working Group, or (b) the Working Group
has made an incorrect technical choice which places the quality
and/or integrity of the Working Group's product(s) in significant
jeopardy. The first issue is a difficulty with Working Group
process; the latter is an assertion of technical error. These two
types of disagreement are quite different, but both are handled by
the same process of review.

A person who disagrees with a Working Group recommendation shall
always first discuss the matter with the Working Group's chair(s),
who may involve other members of the Working Group (or the Working
Group as a whole) in the discussion.

If the disagreement cannot be resolved in this way, any of the
parties involved may bring it to the attention of the Area
Director(s) for the area in which the Working Group is chartered.
The Area Director(s) shall attempt to resolve the dispute.

If the disagreement cannot be resolved by the Area Director(s) any of
the parties involved may then appeal to the IESG as a whole. The
IESG shall then review the situation and attempt to resolve it in a
manner of its own choosing.

If the disagreement is not resolved to the satisfaction of the
parties at the IESG level, any of the parties involved may appeal the
decision to the IAB. The IAB shall then review the situation and
attempt to resolve it in a manner of its own choosing.

The IAB decision is final with respect to the question of whether or
not the Internet Standards Processes have been followed and with
respect to all questions of technical merit.

### Process Failures

This document sets forward procedures required to be followed to
ensure openness and fairness of the Internet Standards Process, and
the technical viability of the standards created. The IESG is the
principal agent of the IETF for this purpose, and it is the IESG that
is charged with ensuring that the required procedures have been
followed, and that any necessary prerequisites to a standards action
have been met.

If an individual should disagree with an action taken by the IESG in
this process, that person should first discuss the issue with the
IESG Chair. If the IESG Chair is unable to satisfy the complainant
then the IESG as a whole should re-examine the action taken, along
with input from the complainant, and determine whether any further
action is needed. The IESG shall issue a report on its review of
the complaint to the IETF.

Should the complainant not be satisfied with the outcome of the IESG
review, an appeal may be lodged to the IAB. The IAB shall then review
the situation and attempt to resolve it in a manner of its own
choosing and report to the IETF on the outcome of its review.

If circumstances warrant, the IAB may direct that an IESG decision be
annulled, and the situation shall then be as it was before the IESG
decision was taken. The IAB may also recommend an action to the IESG,
or make such other recommendations as it deems fit. The IAB may not,
however, pre-empt the role of the IESG by issuing a decision which
only the IESG is empowered to make.

The IAB decision is final with respect to the question of whether or
not the Internet Standards Processes have been followed.

### Questions of Applicable Procedure

Further recourse is available only in cases in which the procedures
themselves (i.e., the procedures described in this document) are
claimed to be inadequate or insufficient to the protection of the
rights of all parties in a fair and open Internet Standards Process.
Claims on this basis may be made to the ISOC Board of
Trustees. The President of the ISOC shall acknowledge
such an appeal within two weeks, and shall at the time of
acknowledgment advise the petitioner of the expected duration of the
Trustees' review of the appeal. The Trustees shall review the
situation in a manner of its own choosing and report to the IETF on
the outcome of its review.

The Trustees' decision upon completion of their review shall be final
with respect to all aspects of the dispute.

### Appeals Procedure

All appeals must include a detailed and specific description of the
facts of the dispute.

All appeals must be initiated within two months of the public
knowledge of the action or decision to be challenged.

At all stages of the appeals process, the individuals or bodies
responsible for making the decisions have the discretion to define
the specific procedures they will follow in the process of making
their decision.

In all cases a decision concerning the disposition of the dispute,
and the communication of that decision to the parties involved, must
be accomplished within a reasonable period of time.

NOTE: These procedures intentionally and explicitly do not
establish a fixed maximum time period that shall be considered
"reasonable" in all cases. The Internet Standards Process places a
premium on consensus and efforts to achieve it, and deliberately
forgoes deterministically swift execution of procedures in favor of
a latitude within which more genuine technical agreements may be
reached.

# External Standards and Specifications {#sec7}

Many standards groups other than the IETF create and publish
standards documents for network protocols and services. When these
external specifications play an important role in the Internet, it is
desirable to reach common agreements on their usage -- i.e., to
establish Internet Standards relating to these external
specifications.

There are two categories of external specifications:

- Open Standards:
Various national and international standards bodies, such as ANSI,
ISO, IEEE, and ITU-T, develop a variety of protocol and service
specifications that are similar to Technical Specifications
defined here. National and international groups also publish
"implementors' agreements" that are analogous to Applicability
Statements, capturing a body of implementation-specific detail
concerned with the practical application of their standards. All
of these are considered to be "open external standards" for the
purposes of the Internet Standards Process.

- Other Specifications:
Other proprietary specifications that have come to be widely used
in the Internet may be treated by the Internet community as if
they were a "standard." Such a specification is not generally
developed in an open fashion, is typically proprietary, and is
controlled by the vendor, vendors, or organization that produced
it.

## Use of External Specifications

To avoid conflict between competing versions of a specification, the
Internet community will not standardize a specification that is
simply an "Internet version" of an existing external specification
unless an explicit cooperative arrangement to do so has been made.
However, there are several ways in which an external specification
that is important for the operation and/or evolution of the Internet
may be adopted for Internet use.

### Incorporation of an Open Standard

An Internet Standard TS or AS may incorporate an open external
standard by reference. For example, many Internet Standards
incorporate by reference the Unicode encoding scheme {{UNICODE}}.
Whenever possible, the referenced specification shall be
available
without restriction or undue fee using
standard Internet applications such as the WWW.

### Incorporation of Other Specifications

Other proprietary specifications may be incorporated by reference
to a version of the specification as long as the proprietor meets
the requirements of {{ipr-requirements}}. If the other proprietary
specification is not widely and readily available, the IESG may
request that it be published as an Informational RFC.

The IESG generally should not favor a particular proprietary
specification over technically equivalent and competing
specification(s) by making any incorporated vendor specification
"required" or "recommended".

### Assumption

An IETF Working Group may start from an external specification and
develop it into an Internet specification. This is acceptable if
(1) the specification is provided to the Working Group in
compliance with the requirements of {{ipr-requirements}}, and (2) change
control has been conveyed to IETF by the original developer of the
specification for the specification or for specifications derived
from the original specification.

# Notices and Record Keeping {#sec8}

Each of the organizations involved in the development and approval
of Internet Standards shall publicly announce, and shall maintain
a publicly accessible record of, every activity in which it
engages, to the extent that the activity represents the
prosecution of any part of the Internet Standards Process. For
purposes of this section, the organizations involved in the
development and approval of Internet Standards includes the IETF,
the IESG, the IAB, all IETF Working Groups, and the Internet
Society Board of Trustees.

For IETF and Working Group meetings announcements shall be made by
electronic mail to the IETF Announce mailing list and shall be
made sufficiently far in advance of the activity to permit all
interested parties to effectively participate. The announcement
shall contain (or provide pointers to) all of the information that
is necessary to support the participation of any interested
individual. In the case of a meeting, for example, the
announcement shall include an agenda that specifies the
standards-related issues that will be discussed.

The formal record of an organization's standards-related activity
shall include at least the following:

- The charter of the organization (or a defining document equivalent
to a charter);

- Complete and accurate minutes of meetings;

- The archives of Working Group electronic mail mailing lists; and

- All written contributions from participants that pertain to the
organization's standards-related activity.

As a practical matter, the formal record of all Internet Standards
Process activities is maintained by the IETF LLC or its designees.
Also, the Working Group chair is
responsible for providing complete and
accurate minutes of all Working Group meetings. Internet-Drafts that
have been removed (for any reason) from the Internet-Drafts
directories shall be archived for the sole
purpose of preserving an historical record of Internet Standards
Process activity and thus are not retrievable except in special
circumstances.

# Varying the Process {#sec9}

This document, which sets out the rules and procedures by which
Internet Standards and related documents are made is itself a product
of the Internet Standards Process (as a BCP, as described in {{sec5}}.)
It replaces a previous version, and in time, is likely itself to
be replaced.

While, when published, this document represents the community's view
of the proper and correct process to follow, and requirements to be
met, to allow for the best possible Internet Standards and BCPs, it
cannot be assumed that this will always remain the case. From time to
time there may be a desire to update it, by replacing it with a new
version. Updating this document uses the same open procedures as are
used for any other BCP.

In addition, there may be situations where following the procedures
leads to a deadlock about a specific specification, or there may be
situations where the procedures provide no guidance. In these cases
it may be appropriate to invoke the variance procedure described
below.

## The Variance Procedure

Upon the recommendation of the responsible IETF Working Group (or, if
no Working Group is constituted, upon the recommendation of an ad hoc
committee), the IESG may enter a particular specification into, or
advance it within, the standards track even though some of the
requirements of this document have not or will not be met. The IESG
may approve such a variance, however, only if it first determines
that the likely benefits to the Internet community are likely to
outweigh any costs to the Internet community that result from
noncompliance with the requirements in this document. In exercising
this discretion, the IESG shall at least consider (a) the technical
merit of the specification, (b) the possibility of achieving the
goals of the Internet Standards Process without granting a variance,
(c) alternatives to the granting of a variance, (d) the collateral
and precedential effects of granting a variance, and (e) the IESG's
ability to craft a variance that is as narrow as possible. In
determining whether to approve a variance, the IESG has discretion to
limit the scope of the variance to particular parts of this document
and to impose such additional restrictions or limitations as it
determines appropriate to protect the interests of the Internet
community.

The proposed variance must detail the problem perceived, explain the
precise provision of this document which is causing the need for a
variance, and the results of the IESG's considerations including
consideration of points (a) through (d) in the previous paragraph.
The proposed variance shall be issued as an Internet Draft. The IESG
shall then issue an extended Last-Call, of no less than 4 weeks, to
allow for community comment upon the proposal.

In a timely fashion after the expiration of the Last-Call period, the
IESG shall make its final determination of whether or not to approve
the proposed variance, and shall notify the IETF of its decision via
electronic mail to the IETF Announce mailing list. If the variance
is approved it shall be forwarded to the RPC with a request
that it be published as a BCP.

This variance procedure is for use when a one-time waiver of some
provision of this document is felt to be required. Permanent changes
to this document shall be accomplished through the normal BCP
process.

The appeals process in {{sec65}} applies to this process.

## Exclusions

No use of this procedure may lower any specified delays, nor exempt
any proposal from the requirements of openness, fairness, or
consensus, nor from the need to keep proper records of the meetings
and mailing list discussions.

Specifically, the following sections of this document must not be
subject of a variance: {{sec51}}, {{sec6}}, {{sec611}} (first paragraph),
{{sec612}}, {{sec63}} (first sentence), {{sec65}} and {{sec9}}.

# Security Considerations

Security issues are not discussed in this memo.

# IANA Considerations

This document has no IANA actions.

# Change Log

## Working group draft

- Draft 0: Adopted by PROCON WG.

- Draft 1: Various GitHub fixes. Improve 7475 obsolescence text. Add wording
about RFC style, output formats, default input; remove text about standards
requiring ASCII. Unindent or remove text blocks. Discuss legacy "Draft
Standard" documents. Tighten IPR requirements on Informational.  Add WG
changelog section.

- Draft 2: Fix link to repository, tweak wording about RFC style and
formats. Clarify that not all discussions must be public.

- Draft 3: Refer to BCP78 for definition of "Contribution."
Clearify procedures for Experimental and Informational.
Clarify ADs can delegate handlling an appeal.
Add AD sponsor as an example of non-WG initiation.
IETF LLC maintains mailing lists anad public records.
Renamed IETF Trust to IETF Intellectual Property Management Corporation.
Various minor editorial/wording changes.

- Draft 4: Remove terminology section; use references on first use when
needed.
Consistency around "Internet Standards Process" term
use and capitalization.
Change "RFC Editor" to "RFC Publication Center."
Put punctuation inside the quotation where necessary.
Avoid "Internet Standards-related" construction
Use subseries consistently for BCP/STD.
Update BCP definition and explain those that affect the standards
process are published on the IETF stream.

- Draft 5: Update Internet-Draft section (with Brian Carpenter).
Remove out-of-scope BCP sentence.

- Draft 6: More wording fixes from Pete caused by #4.
It's RFC Production (not Publication) Center.
BCP and STD may issue new RFC number or not.
A subseries may have multiple RFCs.
When an RFC is obsoleted, it is removed from the subseries and
the obsoleting RFC is added.
Fix text and link to published list of RFCs, STD, etc.

- Draft 7:
Re-order IESG Evaluation to fully undo paragraph shuffling.
Remove added text about when an "update" RFC is in the subseries.
Change RFC Editor link for subseries info.
Add reference to BCP97.

- Draft 8:
Add "standards action requires IESG approval" paragraph.

- Draft 9:
Remove some changes that were decided to be out of scope as
identified by Dan Bernstein and confirmed by Roman.

- Draft 10:
Use Unicode instead of ASCII as external standard example (editorial).
Add references to RFC 8712 and RFC 9920; mention other online fora per RFC 9945
(editorial).
Move "IETF stream needs rough consensus" to the RFC section (4.1) (editorial).
Remove mention of other streams from Experimental (editorial).
All inf/exp drafts get IETSG review (implied by 2026 and 8789).
Remove "directly" from inf/exp publication as its a holdover from
when the RFC Editor (sic) could publish them w/o IESG (editorial).
Edit section headings and move text to avoid re-using the draft
title as a section header (editorial).
Add WG folks to acknowledgements (editorial).

- Draft 11:
Revise wording to say non-standard-track maturity also follow the process
defined in Sec 8 (editorial).
A TS can use elective or optional (editorial).

- Draft 12:
Change wording about IETF last call (editorial).
Remove missed "need not be public" sentence from draft 9 (see above)

## Individual draft

- Draft 0: Translated the nroff source of RFC 2026 into markdown.
The notices in the document at section 12.4 were prefaced with "THIS TEXT
ADDED TO PASS THE IDNITS CHECKS" so that the draft could be published.
The copyright notice is changed to the current one.
Because of this and other boilerplate, some section numbers differ
from the original RFC.

- Draft 1: Add Scott Bradner as co-author. Add Note. Alphabetize
terminology. Minor wording tweaks.

- Draft 2: Clarified Note about the RFC's. More word tweaks.  Remove
bulk of text from the Notices, and point to RFC 2026, to avoid confusion
and pass the idnits checks.

- Draft 3: Incorporated RFC 5378.

- Draft 4: Updated terminology and removed some obvious or old terms.
In some cases this meant minor editorial changes in the body text.

- Draft 5: Add text about RFC 5657 and errata to the intro Note. Incorporate
RFC 5742.

- Draft 6: Incorporate RFC 6410. Moved some text around to make the
new text flow a bit better.

- Draft 7: Incorporate RFC 7100, RFC 7475, and RFC 9282.  Add mention of
the "rfcindex.txt" file.

- Draft 8: Incorporate RFC 7127.

- Draft 9: Incorporate RFC 8789.
Updates (not obsoletes) RFC 5378, RFC 5657, and RFC 7475.

- Draft 10: Incorporate RFC 8179.

- Draft 11: Remove IPR section (RFC 5378 and RFC 8179) and add a pointer
to those RFCs instead.

- Draft 12: Addressed the editorial issues found by the following verified
errata: 523, 524, 1622, 3014, 3095, and 7181. Errata 3095 was marked as
editorial, although it seems to be a semantic change but one that
properly reflects consensus. The following errata were closed by the
conversion to markdown and associated tooling, as they do the right thing:
6658, 6659, 6661, 6671, and 6669.

- Draft 13: Address some pre-adoption issues raised on the WG mailing list.

--- back

# Acknowledgments
{:numbered="false"}

We gratefully acknowledge those who have contributed to the development of
IETF RFC's and the processes that create both the content and documents.  In
particular, we thank the authors of all the documents that updated
{{?RFC2026}}.

We also thank Sandy Ginoza of the Secretariat for sending all the original
RFC sources, and John Klensin for his support and cooperation during the
process of creating this document.

Finally, we thank the members and Chairs of the Working Group for their
suggestions and comments.  In particular, Jari Arkko, Brian Carpenter, Pete
Resnick, Rob Sayre, and David Schinazi made notable contributions. We
also thank Dan Bernstein for his feedback.
