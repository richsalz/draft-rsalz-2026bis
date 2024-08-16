---
title: "The Internet Standards Process"
abbrev: "process"
docname: draft-rsalz-2026bis-latest
submissiontype: IETF
category: bcp
ipr: trust200902
area: General
workgroup: xxxxxxx
keyword: process
stand_alone: yes
smart_quotes: no
obsoletes: 2026, 5378, 5657, 5742, 6410, 7100, 7127, 7475, 8179, 8789, 9282
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
    organization: SOBCO
    email: sob@sobco.com

venue:
 repo: https://github.com/richsalz/draft-rsalz-2026bis.md

normative:

informative:
    RFC2026:
    STDIDX:
      title: STD INDEX
      target: "https://www.ietf.org/rfc/std-index.txt"
      ann: Note that STD1 is no longer published.
    US-ASCII:
      title: Coded Character Set -- 7-Bit American Standard Code for Information Interchange
      author:
      - name: ANSI
      date: "March, 1986"
      ann: "ANSI X3.4-1986"
    BERNE:
      title: "Berne Convention for the Protection of Literary and Artistic Work"
      target: "https://www.wipo.int/treaties/en/ip/berne"

--- abstract

This memo documents the process used by the Internet community for
the standardization of protocols and procedures. It defines the
stages in the standardization process, the requirements for moving a
document between stages and the types of documents used during this
process. It also addresses the intellectual property rights and
copyright issues associated with the standards process.

This document obsoletes RFC2026, RFC5378, RFC5657, RFC5742, RFC6410,
RFC7100, RFC7127, RFC7475, RFC8179, RFC8789, and RFC9282.


--- middle

# Introduction

       NOTE: This document started with the raw text of RFC 2026.  The
       plan is that each version of this Internet-Draft will incorporate
       one of the 10 RFCs that updated the original.  Once all have been
       merged in, we will submit this to the GENDISPATCH working group
       to determine the next steps.

       Specifically, the RFCs to be incorporated are: RFC 5378, RFC
       5657, RFC 5742, RFC 6410, RFC 7100, RFC 7127, RFC 7475, RFC 8179,
       RFC 8789, and RFC 9282.

       RFC 3667 was obsoleted by RFC 3978, which in turn was obsoleted
       by RFC 5378.  RFC 3668 was obsoleted by RFC 3979, which in turn
       was obsoleted by RFC 8179.  RFC 3932 was obsoleted by RFC 5742.
       RFC 3978 was obsoleted by RFC 8179.

This memo documents the process currently used by the Internet
community for the standardization of protocols and procedures. The
Internet Standards process is an activity of the Internet Society
that is organized and managed on behalf of the Internet community by
the Internet Architecture Board (IAB) and the Internet Engineering
Steering Group (IESG).

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

The following terms are used throughout this document.

Area Director
: The manager of an IETF Area. The Area Directors
along with the IETF Chair comprise the Internet Engineering
Steering Group (IESG).

File Transfer Protocol (FTP)
: An Internet application used to
transfer files in a TCP/IP network.

gopher
: An Internet application used to interactively select and
retrieve files in a TCP/IP network.

IETF Area
: A management division within the IETF. An Area consists
of Working Groups related to a general topic such as routing. An
Area is managed by one or two Area Directors.

Internet Architecture Board (IAB)
: An appointed group that assists
in the management of the IETF standards process.

Internet Engineering Steering Group (IESG)
: A group comprised of the
IETF Area Directors and the IETF Chair. The IESG is responsible
for the management, along with the IAB, of the IETF and is the
standards approval board for the IETF.

interoperable
: For the purposes of this document, "interoperable"
means to be able to interoperate over a data communications path.

Last-Call
: A public comment period used to gage the level of
consensus about the reasonableness of a proposed standards action.
See {{sec612}}.

online
: Relating to information made available over the Internet.
When referenced in this document material is said to be online
when it is retrievable without restriction or undue fee using
standard Internet applications such as anonymous FTP, gopher or
the WWW.

Working Group
: A group chartered by the IESG and IAB to work on a
specific specification, set of specifications or topic.

The following acronymns are also used in this document.

ANSI
: American National Standards Institute

ARPA
: (U.S.) Advanced Research Projects Agency

AS
: Applicability Statement

ASCII
: American Standard Code for Information Interchange

FTP
: File Transfer Protocol

IAB
: Internet Architecture Board

IANA
: Internet Assigned Numbers Authority

ICMP
: Internet Control Message Protocol

IEEE
: Institute of Electrical and Electronics Engineers

IESG
: Internet Engineering Steering Group

IETF
: Internet Engineering Task Force

IP
: Internet Protocol

IRSG
: Internet Research Steering Group

IRTF
: Internet Research Task Force

ISO
: International Organization for Standardization

ISOC
: Internet Society

ITU-T
: Telecommunications Standardization sector of the
International Telecommunication Union (ITU), a UN
treaty organization; ITU-T was formerly called CCITT.

MIB
: Management Information Base

OSI
: Open Systems Interconnection

RFC
: Request for Comments

TCP
: Transmission Control Protocol

TS
: Technical Specification

WWW
: World Wide Web


{::boilerplate bcp14-tagged}

# The Internet Standards Process

In outline, the process of creating an Internet Standard is
straightforward: a specification undergoes a period of development
and several iterations of review by the Internet community and
revision based upon experience, is adopted as a Standard by the
appropriate body (see below), and is published. In practice, the
process is more complicated, due to (1) the difficulty of creating
specifications of high technical quality; (2) the need to consider
the interests of all of the affected parties; (3) the importance of
establishing widespread community consensus; and (4) the difficulty
of evaluating the utility of a particular specification for the
Internet community.

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
and its merits debated in open meetings and/or public electronic
mailing lists, and it is made available for review via world-wide
on-line directories.

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
and record keeping {{sec9}} defines a variance process to allow
one-time exceptions to some of the requirements in this document
{{sec10}} presents the rules that are required to protect
intellectual property rights in the context of the development and
use of Internet Standards.

# Internet Standards-Related Publications {#sec2}

## Requests for Comments (RFCs)

Each distinct version of an Internet standards-related specification
is published as part of the "Request for Comments" (RFC) document
series. This archival series is the official publication channel for
Internet standards documents and other publications of the IESG, IAB,
and Internet community. RFCs can be obtained from a number of
Internet hosts using anonymous FTP, gopher, World Wide Web, and other
Internet document-retrieval systems.

The RFC series of documents on networking began in 1969 as part of
the original ARPA wide-area networking (ARPANET) project (see
Appendix A for glossary of acronyms). RFCs cover a wide range of
topics in addition to Internet Standards, from early discussion of
new research concepts to status memos about the Internet. RFC
publication is the direct responsibility of the RFC Editor, under the
general direction of the IAB.

The rules for formatting and submitting an RFC are defined in {{!RFC2223}}.
Every RFC is available in ASCII text. Some RFCs are also available
in other formats. The other versions of an RFC may contain material
(such as diagrams and figures) that is not present in the ASCII
version, and it may be formatted differently.

        A stricter requirement applies to standards-track
        specifications: the ASCII text version is the
        definitive reference, and therefore it must be a
        complete and accurate specification of the standard,
        including all necessary diagrams and illustrations.

The status of Internet protocol and service specifications is
summarized periodically in an RFC entitled "Internet Official
Protocol Standards" [STDIDX]. This RFC shows the level of maturity and
other helpful information for each Internet protocol or service
specification (see {{sec3}}).

Some RFCs document Internet Standards. These RFCs form the 'STD'
subseries of the RFC series {{?RFC1311}}. When a specification has been
adopted as an Internet Standard, it is given the additional label
"STDxxx", but it keeps its RFC number and its place in the RFC
series (see {{sec413}}).

Some RFCs standardize the results of community deliberations about
statements of principle or conclusions about what is the best way to
perform some operations or IETF process function. These RFCs form
the specification has been adopted as a BCP, it is given the
additional label "BCPxxx", but it keeps its RFC number and its place
in the RFC series. (see {{sec5}})

Not all specifications of protocols or services for the Internet
should or will become Internet Standards or BCPs. Such non-standards
track specifications are not subject to the rules for Internet
standardization. Non-standards track specifications may be published
directly as "Experimental" or "Informational" RFCs at the discretion
of the RFC Editor in consultation with the IESG (see {{sec42}}).

        It is important to remember that not all RFCs
        are standards track documents, and that not all
        standards track documents reach the level of
        Internet Standard. In the same way, not all RFCs
        which describe current practices have been given
        the review and approval to become BCPs. See
        {{!RFC-1796} for further information.

## Internet-Drafts {#sec22}

During the development of a specification, draft versions of the
document are made available for informal review and comment by
placing them in the IETF's "Internet-Drafts" directory, which is
replicated on a number of Internet hosts. This makes an evolving
working document readily available to a wide audience, facilitating
the process of review and revision.

An Internet-Draft that is published as an RFC, or that has remained
unchanged in the Internet-Drafts directory for more than six months
without being recommended by the IESG for publication as an RFC, is
simply removed from the Internet-Drafts directory. At any time, an
Internet-Draft may be replaced by a more recent version of the same
specification, restarting the six-month timeout period.

An Internet-Draft is NOT a means of "publishing" a specification;
specifications are published through the RFC mechanism described in
the previous section. Internet-Drafts have no formal status, and are
subject to change or removal at any time.

        Under no circumstances should an Internet-Draft
        be referenced by any paper, report, or Request-
        for-Proposal, nor should a vendor claim compliance
        with an Internet-Draft.

Note: It is acceptable to reference a standards-track specification
that may reasonably be expected to be published as an RFC using the
phrase "Work in Progress" without referencing an Internet-Draft.
This may also be done in a standards track document itself as long
as the specification in which the reference is made would stand as a
complete and understandable document with or without the reference to
the "Work in Progress".

# Internet Standard Specifications {#sec3}

Specifications subject to the Internet Standards Process fall into
one of two categories: Technical Specification (TS) and
Applicability Statement (AS).

## Technical Specification (TS)

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

## Applicability Statement (AS) {#sec32}

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
For example, a TS at Draft Standard level may be referenced by an AS
at the Proposed Standard or Draft Standard level, but not by an AS at
the Standard level.

## Requirement Levels {#sec33}

An AS shall apply one of the following "requirement levels" to each
of the TSs to which it refers:

- Required: Implementation of the referenced TS, as specified by
the AS, is required to achieve minimal conformance. For example,
IP and ICMP must be implemented by all Internet systems using the
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

- Elective: Implementation of the referenced TS is optional
within the domain of applicability of the AS; that is, the AS
creates no explicit necessity to apply the TS. However, a
particular vendor may decide to implement it, or a particular user
may decide that it is a necessity in a specific environment. For
example, the DECNET MIB could be seen as valuable in an
environment where the DECNET protocol is used.

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

The "Official Protocol Standards" RFC (STD1) lists a general
requirement level for each TS, using the nomenclature defined in this
section. This RFC is updated periodically. In many cases, more
detailed descriptions of the requirement levels of particular
protocols and of individual features of the protocols will be found
in appropriate ASs.

# The Internet Standards Track {#sec4}

Specifications that are intended to become Internet Standards evolve
through a set of maturity levels known as the "standards track".
These maturity levels -- "Proposed Standard", "Draft Standard", and
"Standard" -- are defined and discussed in {{sec41}}. The way in
which specifications move along the standards track is described in
{{sec6}}.

Even after a specification has been adopted as an Internet Standard,
further evolution often occurs based on experience and the
recognition of new requirements. The nomenclature and procedures of
Internet standardization provide for the replacement of old Internet
Standards with new ones, and the assignment of descriptive labels to
indicate the status of "retired" Internet Standards. A set of
maturity levels is defined in {{sec42}} to cover these and other
specifications that are not considered to be on the standards track.

## Standards Track Maturity Levels {#sec41}

Internet specifications go through stages of development, testing,
and acceptance. Within the Internet Standards Process, these stages
are formally labeled "maturity levels".

This section describes the maturity levels and the expected
characteristics of specifications at each level.

### Proposed Standard

The entry-level maturity for the standards track is "Proposed
Standard". A specific action by the IESG is required to move a
specification onto the standards track at the "Proposed Standard"
level.

A Proposed Standard specification is generally stable, has resolved
known design choices, is believed to be well-understood, has received
significant community review, and appears to enjoy enough community
interest to be considered valuable. However, further experience
might result in a change or even retraction of the specification
before it advances.

Usually, neither implementation nor operational experience is
required for the designation of a specification as a Proposed
Standard. However, such experience is highly desirable, and will
usually represent a strong argument in favor of a Proposed Standard
designation.

The IESG may require implementation and/or operational experience
prior to granting Proposed Standard status to a specification that
materially affects the core Internet protocols or that specifies
behavior that may have significant operational impact on the
Internet.

A Proposed Standard should have no known technical omissions with
respect to the requirements placed upon it. However, the IESG may
waive this requirement in order to allow a specification to advance
to the Proposed Standard state when it is considered to be useful and
necessary (and timely) even with known technical omissions.

Implementors should treat Proposed Standards as immature
specifications. It is desirable to implement them in order to gain
experience and to validate, test, and clarify the specification.
However, since the content of Proposed Standards may be changed if
problems are found or better solutions are identified, deploying
implementations of such standards into a disruption-sensitive
environment is not recommended.

### Draft Standard

A specification from which at least two independent and interoperable
implementations from different code bases have been developed, and
for which sufficient successful operational experience has been
obtained, may be elevated to the "Draft Standard" level. For the
purposes of this section, "interoperable" means to be functionally
equivalent or interchangeable components of the system or process in
which they are used. If patented or otherwise controlled technology
is required for implementation, the separate implementations must
also have resulted from separate exercise of the licensing process.
Elevation to Draft Standard is a major advance in status, indicating
a strong belief that the specification is mature and will be useful.

The requirement for at least two independent and interoperable
implementations applies to all of the options and features of the
specification. In cases in which one or more options or features
have not been demonstrated in at least two interoperable
implementations, the specification may advance to the Draft Standard
level only if those options or features are removed.

The Working Group chair is responsible for documenting the specific
implementations which qualify the specification for Draft or Internet
Standard status along with documentation about testing of the
interoperation of these implementations. The documentation must
include information about the support of each of the individual
options and features. This documentation should be submitted to the
Area Director with the protocol action request. (see {{sec6}})

A Draft Standard must be well-understood and known to be quite
stable, both in its semantics and as a basis for developing an
implementation. A Draft Standard may still require additional or
more widespread field experience, since it is possible for
implementations based on Draft Standard specifications to demonstrate
unforeseen behavior when subjected to large-scale use in production
environments.

A Draft Standard is normally considered to be a final specification,
and changes are likely to be made only to solve specific problems
encountered. In most circumstances, it is reasonable for vendors to
deploy implementations of Draft Standards into a disruption sensitive
environment.

### Internet Standard {#sec413}

A specification for which significant implementation and successful
operational experience has been obtained may be elevated to the
Internet Standard level. An Internet Standard (which may simply be
referred to as a Standard) is characterized by a high degree of
technical maturity and by a generally held belief that the specified
protocol or service provides significant benefit to the Internet
community.

A specification that reaches the status of Standard is assigned a
number in the STD series while retaining its RFC number.

## Non-Standards Track Maturity Levels {#sec42}

Not every specification is on the standards track. A specification
may not be intended to be an Internet Standard, or it may be intended
for eventual standardization but not yet ready to enter the standards
track. A specification may have been superseded by a more recent
Internet Standard, or have otherwise fallen into disuse or disfavor.

Specifications that are not on the standards track are labeled with
one of three "off-track" maturity levels: "Experimental",
"Informational", or "Historic". The documents bearing these labels
are not Internet Standards in any sense.

### Experimental

The "Experimental" designation typically denotes a specification that
is part of some research or development effort. Such a specification
is published for the general information of the Internet technical
community and as an archival record of the work, subject only to
editorial considerations and to verification that there has been
adequate coordination with the standards process (see below). An
Experimental specification may be the output of an organized Internet
research effort (e.g., a Research Group of the IRTF), an IETF Working
Group, or it may be an individual contribution.

### Informational

An "Informational" specification is published for the general
information of the Internet community, and does not represent an
Internet community consensus or recommendation. The Informational
designation is intended to provide for the timely publication of a
very broad range of responsible informational documents from many
sources, subject only to editorial considerations and to verification
that there has been adequate coordination with the standards process
(see {{sec423}}).

Specifications that have been prepared outside of the Internet
community and are not incorporated into the Internet Standards
Process by any of the provisions of {{sec10}} may be published as
Informational RFCs, with the permission of the owner and the
concurrence of the RFC Editor.

### Procedures for Experimental and Informational RFCs {#sec423}

Unless they are the result of IETF Working Group action, documents
intended to be published with Experimental or Informational status
should be submitted directly to the RFC Editor. The RFC Editor will
publish any such documents as Internet-Drafts which have not already
been so published. In order to differentiate these Internet-Drafts
they will be labeled or grouped in the I-D directory so they are
easily recognizable. The RFC Editor will wait two weeks after this
publication for comments before proceeding further. The RFC Editor
is expected to exercise his or her judgment concerning the editorial
suitability of a document for publication with Experimental or
Informational status, and may refuse to publish a document which, in
the expert opinion of the RFC Editor, is unrelated to Internet
activity or falls below the technical and/or editorial standard for
RFCs.

To ensure that the non-standards track Experimental and Informational
designations are not misused to circumvent the Internet Standards
Process, the IESG and the RFC Editor have agreed that the RFC Editor
will refer to the IESG any document submitted for Experimental or
Informational publication which, in the opinion of the RFC Editor,
may be related to work being done, or expected to be done, within the
IETF community. The IESG shall review such a referred document
within a reasonable period of time, and recommend either that it be
published as originally submitted or referred to the IETF as a
contribution to the Internet Standards Process.

If (a) the IESG recommends that the document be brought within the
IETF and progressed within the IETF context, but the author declines
to do so, or (b) the IESG considers that the document proposes
something that conflicts with, or is actually inimical to, an
established IETF effort, the document may still be published as an
Experimental or Informational RFC. In these cases, however, the IESG
may insert appropriate "disclaimer" text into the RFC either in or
immediately following the "Status of this Memo" section in order to
make the circumstances of its publication clear to readers.

Documents proposed for Experimental and Informational RFCs by IETF
Working Groups go through IESG review. The review is initiated using
the process described in {{sec611}}.

### Historic

A specification that has been superseded by a more recent
specification or is for any other reason considered to be obsolete is
assigned to the "Historic" level. (Purists have suggested that the
word should be "Historical"; however, at this point the use of
"Historic" is historical.)

Note: Standards track specifications normally must not depend on
other standards track specifications which are at a lower maturity
level or on non standards track specifications other than referenced
specifications from other standards bodies. (See {{sec7}}.)

# Best Current Practice (BCP) RFCs {#sec5}

The BCP subseries of the RFC series is designed to be a way to
standardize practices and the results of community deliberations. A
BCP document is subject to the same basic set of procedures as
standards track documents and thus is a vehicle by which the IETF
community can define and ratify the community's best current thinking
on a statement of principle or on what is believed to be the best way
to perform some operations or IETF process function.

Historically Internet standards have generally been concerned with
the technical specifications for hardware and software required for
computer communication across interconnected networks. However,
since the Internet itself is composed of networks operated by a great
variety of organizations, with diverse goals and rules, good user
service requires that the operators and administrators of the
Internet follow some common guidelines for policies and operations.
While these guidelines are generally different in scope and style
from protocol standards, their establishment needs a similar process
for consensus building.

While it is recognized that entities such as the IAB and IESG are
composed of individuals who may participate, as individuals, in the
technical work of the IETF, it is also recognized that the entities
themselves have an existence as leaders in the community. As leaders
in the Internet technical community, these entities should have an
outlet to propose ideas to stimulate work in a particular area, to
raise the community's sensitivity to a certain issue, to make a
statement of architectural principle, or to communicate their
thoughts on other matters. The BCP subseries creates a smoothly
structured way for these management entities to insert proposals into
the consensus-building machinery of the IETF while gauging the
community's view of that issue.

Finally, the BCP series may be used to document the operation of the
IETF itself. For example, this document defines the IETF Standards
Process and is published as a BCP.

## BCP Review Process {#sec51}

Unlike standards-track documents, the mechanisms described in BCPs
are not well suited to the phased roll-in nature of the three stage
standards track and instead generally only make sense for full and
immediate instantiation.

The BCP process is similar to that for proposed standards. The BCP
is submitted to the IESG for review, (see {{sec611}}) and the
existing review process applies, including a Last-Call on the IETF
Announce mailing list. However, once the IESG has approved the
document, the process ends and the document is published. The
resulting document is viewed as having the technical approval of the
IETF.

Specifically, a document to be considered for the status of BCP must
undergo the procedures outlined in {{sec61}}, and {{sec64}} of this
document. The BCP process may be appealed according to the procedures
in {{sec65}}.

Because BCPs are meant to express community consensus but are arrived
at more quickly than standards, BCPs require particular care.
Specifically, BCPs should not be viewed simply as stronger
Informational RFCs, but rather should be viewed as documents suitable
for a content different from Informational RFCs.

A specification, or group of specifications, that has, or have been
approved as a BCP is assigned a number in the BCP series while
retaining its RFC number(s).

# The Internet Standards Process {#sec6}

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

## Standards Actions {#sec61}

A "standards action" -- entering a particular specification into,
advancing it within, or removing it from, the standards track -- must
be approved by the IESG.

### Initiation of Action {#sec611}

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

### IESG Review and Approval {#sec612}

The IESG shall determine whether or not a specification submitted to
it according to {{sec611}}} satisfies the applicable criteria for
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

The Last-Call period shall be no shorter than two weeks except in
those cases where the proposed standards action was not initiated by
an IETF Working Group, in which case the Last-Call period shall be no
shorter than four weeks. If the IESG believes that the community
interest would be served by allowing more time for comment, it may
decide on a longer Last-Call period or to explicitly lengthen a
current Last-Call period.

The IESG is not bound by the action recommended when the
specification was submitted. For example, the IESG may decide to
consider the specification for publication in a different category
than that requested. If the IESG determines this before the Last-
Call is issued then the Last-Call should reflect the IESG's view.
The IESG could also decide to change the publication category based
on the response to a Last-Call. If this decision would result in a
specification being published at a "higher" level than the original
Last-Call was for, a new Last-Call should be issued indicating the
IESG recommendation. In addition, the IESG may decide to recommend
the formation of a new Working Group in the case of significant
controversy in response to a Last-Call for specification not
originating from an IETF Working Group.

In a timely fashion after the expiration of the Last-Call period, the
IESG shall make its final determination of whether or not to approve
the standards action, and shall notify the IETF of its decision via
electronic mail to the IETF Announce mailing list.

### Publication

If a standards action is approved, notification is sent to the RFC
Editor and copied to the IETF with instructions to publish the
specification as an RFC. The specification shall at that point be
removed from the Internet-Drafts directory.

An official summary of standards actions completed and pending shall
appear in each issue of the Internet Society's newsletter. This
shall constitute the "publication of record" for Internet standards
actions.

The RFC Editor shall publish periodically an "Internet Official
Protocol Standards" RFC [STDIDX], summarizing the status of all Internet
protocol and service specifications.

## Advancing in the Standards Track

The procedure described in {{sec61}} is followed for each action
that attends the advancement of a specification along the standards
track.

A specification shall remain at the Proposed Standard level for at
least six (6) months.

A specification shall remain at the Draft Standard level for at least
four (4) months, or until at least one IETF meeting has occurred,
whichever comes later.

These minimum periods are intended to ensure adequate opportunity for
community review without severely impacting timeliness. These
intervals shall be measured from the date of publication of the
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
cases, the IESG or RFC Editor may be asked to republish the RFC (with
a new number) with corrections, and this will not reset the minimum
time-at-level clock.

When a standards-track specification has not reached the Internet
Standard level but has remained at the same maturity level for
twenty-four (24) months, and every twelve (12) months thereafter
until the status is changed, the IESG shall review the viability of
the standardization effort responsible for that specification and the
usefulness of the technology. Following each such review, the IESG
shall approve termination or continuation of the development effort,
at the same time the IESG shall decide to maintain the specification
at the same maturity level or to move it to Historic status. This
decision shall be communicated to the IETF by electronic mail to the
IETF Announce mailing list to allow the Internet community an
opportunity to comment. This provision is not intended to threaten a
legitimate and active Working Group effort, but rather to provide an
administrative mechanism for terminating a moribund effort.

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
Internet standards issues that cannot be resolved through the normal
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
not the Internet standards procedures have been followed and with
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
ISEG Chair. If the IESG Chair is unable to satisfy the complainant
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
not the Internet standards procedures have been followed.

### Questions of Applicable Procedure

Further recourse is available only in cases in which the procedures
themselves (i.e., the procedures described in this document) are
claimed to be inadequate or insufficient to the protection of the
rights of all parties in a fair and open Internet Standards Process.
Claims on this basis may be made to the Internet Society Board of
Trustees. The President of the Internet Society shall acknowledge
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
foregoes deterministically swift execution of procedures in favor of
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
they were a "standards". Such a specification is not generally
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
incorporate by reference the ANSI standard character set "US-ASCII"
{{US-ASCII}}. Whenever possible, the referenced specification shall be
available online.

### Incorporation of Other Specifications

Other proprietary specifications may be incorporated by reference
to a version of the specification as long as the proprietor meets
the requirements of {{sec10}}. If the other proprietary
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
compliance with the requirements of {{sec10}}, and (2) change
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
announcement shall include an agenda that specifies the standards-
related issues that will be discussed.

The formal record of an organization's standards-related activity
shall include at least the following:

- The charter of the organization (or a defining document equivalent
to a charter);

- Complete and accurate minutes of meetings;

- The archives of Working Group electronic mail mailing lists; and

- All written contributions from participants that pertain to the
organization's standards-related activity.

As a practical matter, the formal record of all Internet Standards
Process activities is maintained by the IETF Secretariat, and is the
responsibility of the IETF Secretariat except that each IETF Working
Group is expected to maintain their own email list archive and must
make a best effort to ensure that all traffic is captured and
included in the archives. Also, the Working Group chair is
responsible for providing the IETF Secretariat with complete and
accurate minutes of all Working Group meetings. Internet-Drafts that
have been removed (for any reason) from the Internet-Drafts
directories shall be archived by the IETF Secretariat for the sole
purpose of preserving an historical record of Internet standards
activity and thus are not retrievable except in special
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
is approved it shall be forwarded to the RFC Editor with a request
that it be published as a BCP.

This variance procedure is for use when a one-time waving of some
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
subject of a variance: {{sec51}}, {{sec61}}, {{sec611}} (first paragraph),
{{sec612}}, {{sec63}} (first sentence), {{sec65}} and {{sec9}}.

# Intellectual Property Rights {#sec10}

## General Policy

In all matters of intellectual property rights and procedures, the
intention is to benefit the Internet community and the public at
large, while respecting the legitimate rights of others.

## Confidentiality Obligations

No contribution that is subject to any requirement of confidentiality
or any restriction on its dissemination may be considered in any part
of the Internet Standards Process, and there must be no assumption of
any confidentiality obligation with respect to any such contribution.

## Rights and Permissions

In the course of standards work, the IETF receives contributions in
various forms and from many persons. To best facilitate the
dissemination of these contributions, it is necessary to understand
any intellectual property rights (IPR) relating to the contributions.

### All Contributions

By submission of a contribution, each person actually submitting the
contribution is deemed to agree to the following terms and conditions
on his own behalf, on behalf of the organization (if any) he
represents and on behalf of the owners of any propriety rights in the
contribution.. Where a submission identifies contributors in
addition to the contributor(s) who provide the actual submission, the
actual submitter(s) represent that each other named contributor was
made aware of and agreed to accept the same terms and conditions on
his own behalf, on behalf of any organization he may represent and
any known owner of any proprietary rights in the contribution.

- Some works (e.g. works of the U.S. Government) are not subject to
copyright. However, to the extent that the submission is or may
be subject to copyright, the contributor, the organization he
represents (if any) and the owners of any proprietary rights in
the contribution, grant an unlimited perpetual, non-exclusive,
royalty-free, world-wide right and license to the ISOC and the
IETF under any copyrights in the contribution. This license
includes the right to copy, publish and distribute the
contribution in any way, and to prepare derivative works that are
based on or incorporate all or part of the contribution, the
license to such derivative works to be of the same scope as the
license of the original contribution.

- The contributor acknowledges that the ISOC and IETF have no duty
to publish or otherwise use or disseminate any contribution.

- The contributor grants permission to reference the name(s) and
address(es) of the contributor(s) and of the organization(s) he
represents (if any).

- The contributor represents that contribution properly acknowledge
major contributors.

- The contribuitor, the organization (if any) he represents and the
owners of any proprietary rights in the contribution, agree that
no information in the contribution is confidential and that the
ISOC and its affiliated organizations may freely disclose any
information in the contribution.

- The contributor represents that he has disclosed the existence of
any proprietary or intellectual property rights in the
contribution that are reasonably and personally known to the
contributor. The contributor does not represent that he
personally knows of all potentially pertinent proprietary and
intellectual property rights owned or claimed by the organization
he represents (if any) or third parties.

- The contributor represents that there are no limits to the
contributor's ability to make the grants acknowledgments and
agreements above that are reasonably and personally known to the
contributor.

By ratifying this description of the IETF process the Internet
Society warrants that it will not inhibit the traditional open and
free access to IETF documents for which license and right have
been assigned according to the procedures set forth in this
section, including Internet-Drafts and RFCs. This warrant is
perpetual and will not be revoked by the Internet Society or its
successors or assigns.

### Standards Track Documents

- Where any patents, patent applications, or other proprietary
rights are known, or claimed, with respect to any specification on
the standards track, and brought to the attention of the IESG, the
IESG shall not advance the specification without including in the
document a note indicating the existence of such rights, or
claimed rights. Where implementations are required before
advancement of a specification, only implementations that have, by
statement of the implementors, taken adequate steps to comply with
any such rights, or claimed rights, shall be considered for the
purpose of showing the adequacy of the specification.

- The IESG disclaims any responsibility for identifying the
existence of or for evaluating the applicability of any claimed
copyrights, patents, patent applications, or other rights in the
fulfilling of the its obligations under (A), and will take no
position on the validity or scope of any such rights.

- Where the IESG knows of rights, or claimed rights under (A), the
IETF Executive Director shall attempt to obtain from the claimant
of such rights, a written assurance that upon approval by the IESG
of the relevant Internet standards track specification(s), any
party will be able to obtain the right to implement, use and
distribute the technology or works when implementing, using or
distributing technology based upon the specific specification(s)
under openly specified, reasonable, non-discriminatory terms.
The Working Group proposing the use of the technology with respect
to which the proprietary rights are claimed may assist the IETF
Executive Director in this effort. The results of this procedure
shall not affect advancement of a specification along the
standards track, except that the IESG may defer approval where a
delay may facilitate the obtaining of such assurances. The
results will, however, be recorded by the IETF Executive Director,
and made available. The IESG may also direct that a summary of
the results be included in any RFC published containing the
specification.

### Determination of Reasonable and Non-discriminatory Terms

The IESG will not make any explicit determination that the assurance
of reasonable and non-discriminatory terms for the use of a
technology has been fulfilled in practice. It will instead use the
normal requirements for the advancement of Internet Standards to
verify that the terms for use are reasonable. If the two unrelated
implementations of the specification that are required to advance
from Proposed Standard to Draft Standard have been produced by
different organizations or individuals or if the "significant
implementation and successful operational experience" required to
advance from Draft Standard to Standard has been achieved the
assumption is that the terms must be reasonable and to some degree,
non-discriminatory. This assumption may be challenged during the
Last-Call period.

## Notices

Standards track documents shall include the following notice:

    The IETF takes no position regarding the validity or scope of
        ...content elided to avoid confusion; please see
        section 10.4 of RFC 2026...
    obtained from the IETF Secretariat.

The IETF encourages all interested parties to bring to its
attention, at the earliest possible time, the existence of any
intellectual property rights pertaining to Internet Standards.
For this purpose, each standards document shall include the
following invitation:

    The IETF invites any interested party to bring to its attention
        ...content elided to avoid confusion; please see
        section 10.4 of RFC 2026...
    information to the IETF Executive Director.

The following copyright notice and disclaimer shall be included
in all ISOC standards-related documentation:

    Copyright (C) The Internet Society (date). All Rights Reserved.

    This document and translations of it may be copied and furnished
        ...content elided to avoid confusion; please see
        section 10.4 of RFC 2026...
    PARTICULAR PURPOSE.

Where the IESG is aware at the time of publication of proprietary rights
claimed with respect to a standards track document, or the technology
described or referenced therein, such document shall contain the
following notice:

    The IETF has been notified of intellectual property rights
        ...content elided to avoid confusion; please see
        section 10.4 of RFC 2026...
    of claimed rights.

# Security Considerations

Security issues are not discussed in this memo.

# IANA Considerations

This document has no IANA actions.

# Change Log

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

--- back

# Acknowledgments
{:numbered="false"}

We gratefully acknowledge those who have contributed to the development of
IETF RFC's and the processes that create both the content and documents.  In
particular, we thank the authors of all the documents that updated
{{RFC2026}}.

We also thank Sandy Ginoza of the Secretariat for sending all the
original RFC sources.