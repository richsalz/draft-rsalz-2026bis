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
obsoletes: 2026, 6410, 7100, 7127, 8179, 8789, 9282
updates: 5378, 5657, 7475
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
 repo: https://github.com/richsalz/draft-rsalz-2026bis

normative:

informative:
    bis2418: I-D.draft-rsalz-2418bis
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

This document obsoletes RFC2026, RFC5657, RFC6410,
RFC7100, RFC7127, RFC7475, RFC8179, RFC8789, and RFC9282.
It updates RFC5378, RFC5657.
It also updated RFC7475, and with {{bis2418}}, obsoletes it.


--- middle

# Introduction

       NOTE: This document started with the raw text of RFC 2026.  The
       plan is that each version of this Internet-Draft will incorporate
       one of the 10 RFCs that updated the original.  Once all have been
       merged in, we will submit this to the GENDISPATCH working group
       to determine the next steps.

       Specifically, the RFCs to be incorporated are: RFC 5378,
       RFC 6410, RFC 7100, RFC 7127, RFC 7475, RFC 8179,
       RFC 8789, and RFC 9282.

       RFC 3667 was obsoleted by RFC 3978, which in turn was obsoleted
       by RFC 5378.  RFC 3668 was obsoleted by RFC 3979, which in turn
       was obsoleted by RFC 8179.  RFC 3932 was obsoleted by RFC 5742.
       RFC 3978 was obsoleted by RFC 8179.  RFC 5657 became not relevant
       because of RFC 6410, which is also emphasized by RFC 7127.

       If this document gets adopted by a Working Group, the errata for
       all of the above-mentioned RFCs should be reviewed.

This memo documents the process currently used by the Internet
community for the standardization of protocols and procedures. The
Internet Standards process is an activity of the Internet Society (ISOC)
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

The process described here only applies to the IETF RFC stream.  See
{{?RFC4844}} for the definition of the streams and {{?RFC5742}} for a
description of the IESG responsibilities related to those streams.


## Terminology

{::boilerplate bcp14info}

The following terms are used throughout this document.
For more details about the organizations related to the IETF, see
{{!RFC9281, Section 3}}.

Alternate Stream
:  The IAB Document Stream, the IRTF Document Stream, and the Independent
Submission Stream, each as defined in {{?RFC8729, Section 5.1}}, along with
any future non-IETF streams that might be defined.

Area Director
: The manager of an IETF Area.

ARPA
: Advanced Research Projects Agency; an agency of the US
Department of Defense.

Blanket IPR Statement or Blanket Disclosure
: See {{sec543}}.

Contribution
: Any submission to the IETF intended by the Contributor for publication as
all or part of an Internet-Draft or RFC and any statement made within the
context of an IETF activity, in each case that is intended to affect the IETF
Standards Process or that is related to the activity of an Alternate Stream
that has adopted this policy.

Such statements include oral statements, as well as written and electronic
communications, which are addressed to:

- Any IETF plenary session,

- Any IETF Working Group (WG; see {{?BCP25}}) or portion thereof or
any WG chair on behalf of the relevant WG,

- Any IETF "birds of a feather" (BOF) session or portion thereof,

- WG design teams (see {{BCP25}}) and other design teams that intend
to deliver an output to IETF, or portions thereof,

- The IESG, or any member thereof on behalf of the IESG,

- The IAB, or any member thereof on behalf of the IAB,

- Any IETF mailing list, web site, chat room, or discussion board
operated by or under the auspices of the IETF, including the
IETF list itself,

- The RFC Editor or the Internet-Drafts function.

Statements made outside of an IETF session, mailing list, or other function,
or that are clearly not intended to be input to an IETF activity, group, or
function, are not Contributions in the context of this document.  And while
the IETF's IPR rules apply in all cases, not all presentations represent a
Contribution.  For example, many invited plenary, area-meeting, or research
group presentations will cover useful background material, such as general
discussions of existing Internet technology and products, and will not be a
Contribution.  (Some such presentations can represent a Contribution as well,
of course).  Throughout this document, the term "written Contribution" is
used.  For purposes of this document, "written" means reduced to a written or
visual form in any language and any media, permanent or temporary, including
but not limited to traditional documents, email messages, discussion board
postings, slide presentations, text messages, instant messages, and
transcriptions of oral statements.

Contributor
: An individual submitting a Contribution.

Copyright
: The legal right granted to an author in a document or other work of
authorship under applicable law.  A "copyright" is not equivalent to a "right
to copy".  Rather a copyright encompasses all of the exclusive rights that an
author has in a work, such as the rights to copy, publish, distribute and
create derivative works of the work.  An author often cedes these rights to
his or her employer or other parties as a condition of employment or
compensation.

Covers or Covered
: A valid claim of a patent or a patent application (including a provisional
patent application) in any jurisdiction, or any other Intellectual Property
Right, would necessarily be infringed by the exercise of a right (e.g.,
making, using, selling, importing, distribution, copying, etc.) with respect
to an Implementing Technology.  For purposes of this definition, "valid
claim" means a claim of any unexpired patent or patent application which
shall not have been withdrawn, cancelled, or disclaimed, nor held invalid by
a court of competent jurisdiction in an unappealed or unappealable decision.

General Disclosure
: See {{general-disclosures}}.

IETF
: In the context of this document, the IETF includes all individuals who
participate in meetings, working groups, mailing lists, functions, and other
activities that are organized or initiated by ISOC,
the IESG, or the IAB
under the general designation of the Internet Engineering Task Force (IETF),
but solely to the extent of such participation.

IETF Area
: A management division within the IETF. An Area consists
of Working Groups related to a general topic such as routing. An
Area is managed by one or more Area Directors.

IETF Documents
: RFCs and Internet-Drafts that are published as
part of the IETF Standards Process.  These are also referred to as
"IETF Stream Documents" as defined in {{RFC8729, Section 5.1.1}}.

IETF Standards Process
: The activities undertaken by the IETF in any of the settings described
in the above definition of Contribution.  The IETF Standards Process may
include participation in activities and publication of documents that
are not directed toward the development of IETF standards or
specifications, such as the development and publication of Informational
and Experimental documents (see {{sec4}}).

IETF Trust
: A trust established under the laws of the Commonwealth of Virginia, USA, in
order to hold and administer intellectual property rights for the benefit of
the IETF.

Implementing Technology
: A technology that implements an IETF specification or standard.

Indirect Contributor
: Any person who has materially or substantially contributed to a
Contribution without being personally involved in its submission to the IETF.

Internet-Draft
: A document used in the IETF and RFC Editor
processes, as described in {{sec2}}.

Internet Engineering Steering Group (IESG)
: A group comprised of the
IETF Area Directors and the IETF Chair. The IESG is responsible
for the management, along with the IAB, of the IETF and is the
standards approval board for the IETF.

interoperable
: For the purposes of this document, "interoperable"
means to be able to interoperate over a data communications path.

IPR or Intellectual Property Rights
: Means a patent, utility model, or similar right that may Cover an
Implementing Technology, whether such rights arise from a registration or
renewal thereof, or an application therefore, in each case anywhere in the
world.  See {{use-trademarks}} for a discussion of trademarks.

Last-Call
: A public comment period used to gauge the level of
consensus about the reasonableness of a proposed standards action.
See {{sec612}}.

Legend Instructions
: The standardized text that is maintained by the IETF Trust and is included
in IETF Documents and the instructions and requirements for including that
standardized text in IETF Documents.  The text and instructions are posted
from time to time at the
[Trust Legal Provisions](https://trustee.ietf.org/documents/trust-legal-provisions/)

Participating in an IETF discussion or activity
: Making a Contribution, as described above, or in any other way acting in
order to influence the outcome of a discussion relating to the IETF Standards
Process.  Without limiting the generality of the foregoing, acting as a
Working Group Chair or Area Director constitutes "Participating" in all
activities of the relevant working group(s) he or she is responsible for in
an area.  "Participant" and "IETF Participant" mean any individual
Participating in an IETF discussion or activity.

RFC
: The basic publication series for the IETF.

Reasonably and personally known
: Something an individual knows personally or, because of the job the
individual holds, would reasonably be expected to know.  This wording is used
to indicate that an organization cannot purposely keep an individual in the
dark about patents or patent applications just to avoid the disclosure
requirement.  But this requirement should not be interpreted as requiring the
IETF Contributor or Participant (or his or her represented organization, if
any) to perform a patent search to find applicable IPR.

Working Group
: A group chartered by the IESG and IAB to work on a
specific specification, set of specifications or topic.

# The Internet Standards Process {#std-process}

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
and the Internet community. RFCs can be obtained from a number of
Interenet hosts using standard Internet applications such as the WWW.

The RFC series of documents on networking began in 1969 as part of
the original ARPA wide-area networking (ARPANET) project.
RFCs cover a wide range of
topics in addition to Internet Standards, from early discussion of
new research concepts to status memos about the Internet.
For information about RFC publication, see {{?RFC9280}}.

The rules for formatting and submitting an RFC are defined in {{!RFC7322}}.
Every RFC is available in ASCII text. Some RFCs are also available
in other formats. The other versions of an RFC may contain material
(such as diagrams and figures) that is not present in the ASCII
version, and it may be formatted differently.

        A stricter requirement applies to standards-track
        specifications: the ASCII text version is the
        definitive reference, and therefore it must be a
        complete and accurate specification of the standard,
        including all necessary diagrams and illustrations.

Some RFCs document Internet Standards. These RFCs form the 'STD'
subseries of the RFC series {{?RFC1311}}. When a specification has been
adopted as an Internet Standard, it is given the additional label
"STDxxx", but it keeps its RFC number and its place in the RFC
series (see {{sec413}}).
The status of Internet protocol and service specifications is available
from the [RFC Index](https://www.rfc-editor.org/rfc-index.txt) in the
RFC repository.

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
        {{!RFC1796} for further information.

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

## Requirement Levels {#sec33}

An AS shall apply one of the following "requirement levels" to each
of the TSs to which it refers:

- Required: Implementation of the referenced TS, as specified by
the AS, is required to achieve minimal conformance. For example,
IP and the Internet Control Message Protocl (ICMP) must be implemented
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

- Elective: Implementation of the referenced TS is optional
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
Standard".  A specific action by the IESG is required to move a
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
assigned a number in the STD series while retaining its RFC number.

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
research effort (e.g., a Research Group of the Internet Research Task Force)
an IETF Working
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

For classification as an Internet Standard, the request for reclassification
must include an explanation of how the following criteria have
been met:

1. There are at least two independent interoperating implementations
with widespread deployment and successful operational experience.
Although not required by the IETF Standards Process, {{?RFC5657}}
can be helpful to conduct interoperability testing.

2. There are no errata against the specification that would cause a
new implementation to fail to interoperate with deployed ones.

3. There are no unused features in the specification that greatly
increase implementation complexity.

4. If the technology required to implement the specification
requires patented or otherwise controlled technology, then the
set of implementations must demonstrate at least two independent,
separate and successful uses of the licensing process.

### IESG Review and Approval {#sec612}

The IESG shall determine whether or not a specification submitted to
it according to {{sec611}} satisfies the applicable criteria for
the recommended action (see {{sec41}} and {{sec42}}), and shall in
addition determine whether or not the technical quality and clarity
of the specification is consistent with that expected for the
maturity level to which the specification is recommended.

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

For a Proposed Standard,
the Last-Call period shall be no shorter than two weeks except in
those cases where the proposed standards action was not initiated by
an IETF Working Group, in which case the Last-Call period shall be no
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
reclassification, the RFC will be reclassified without publication of
a new RFC.

In a timely fashion after the expiration of the Last-Call period, the
IESG shall make its final determination of whether or not to approve
the standards action, and shall notify the IETF of its decision via
electronic mail to the IETF Announce mailing list.

In no event shall a document be published on the IETF Stream
without IETF consensus.

### Publication

If a standards action is approved, notification is sent to the RFC
Editor and copied to the IETF with instructions to publish the
specification as an RFC. The specification shall at that point be
removed from the Internet-Drafts directory.

## Advancing in the Standards Track

The procedure described in {{sec61}} is followed for each action
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
cases, the IESG or RFC Editor may be asked to republish the RFC (with
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
available
without restriction or undue fee using
standard Internet applications such as the WWW.

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

This section is not intended as legal advice. Readers are advised
to consult their own legal advisors if they would like a legal
interpretation of their rights or the rights of the IETF Trust
{{?RFC8714}} in any Contributions they make.

The IETF policies about Intellectual Property Rights (IPR), such as
patent rights, relative to technologies developed in the IETF are
designed to ensure that IETF working groups and Participants have as
much information as possible about any IPR constraints on a technical
proposal as early as possible in the development process.  The
policies are intended to benefit the Internet community and the
public at large, while respecting the legitimate rights of IPR
holders.  This document details the IETF policies concerning IPR
related to technology worked on within the IETF.  It also describes
the objectives that the policies are designed to meet.

There are three basic principles regarding how the IETF deals with
claims of Intellectual Property Rights:

1. The IETF will make no determination about the validity of any
particular IPR claim.

2. The IETF, following normal processes, can decide to use technology
for which IPR disclosures have been made if it decides that such a
use is warranted.

3. In order for a working group and the rest of the IETF to have
the information needed to make an informed decision about the use
of a particular technology, all those contributing to the working
group's discussions must disclose the existence of any IPR the
Contributor or any other IETF Participant believes Covers or may
ultimately Cover the technology under discussion.  This applies to
both Contributors and other Participants, and applies whether they
contribute in person, via email, or by other means.  The
requirement applies to all IPR of the Participant, the
Participant's employer, sponsor, or others represented by the
Participant that are reasonably and personally known to the
Participant.  No patent search is required.

In all matters relating to Intellectual Property Rights, the intent
is to benefit the Internet community and the public at large, while
respecting the legitimate rights of others.  The disclosures required
by this policy are intended to help IETF working groups define
superior technical solutions with the benefit of as much information
as reasonably possible about potential IPR claims relating to
technologies under consideration.

## Rights and Permissions in Contributions

By submission of a Contribution, each person actually submitting the
Contribution, and each named co-Contributor, is deemed to agree to
the following terms and conditions on his or her own behalf and on
behalf of the organizations the Contributor represents or is
sponsored by (if any) when submitting the Contribution.

## Obligations on Participants

By Participating in the IETF, each Participant is deemed to agree to
comply with all requirements of this RFC that relate to Participation
in IETF activities.  Without limiting the foregoing, each Participant
that is a Contributor makes the following representations to the IETF:

1. Such Contributor represents that he or she has made or will
promptly make all disclosures required by {{ipr-contrib}} of this
document.

2. Such Contributor represents that there are no limits to the
Contributor's ability to make the grants, acknowledgments, and
agreements herein that are reasonably and personally known to the
Contributor.

## Application to Non-IETF Stream Documents

This document has been developed for the benefit and use of the IETF
community.  As such, the rules set forth herein apply to all
Contributions and IETF Documents that are in the "IETF Document
Stream" as defined in {{RFC8729, Section 5.1.1}} (i.e., those that are
contributed, developed, edited, and published as part of the IETF
Standards Process).

The rules that apply to documents in Alternate Streams are
established by the managers of those Alternate Streams (currently the
Internet Architecture Board (IAB), Internet Research Steering Group
(IRSG), and Independent Submission Editor, as specified in {{RFC8729}}).
These managers may elect, through their own internal processes, to
cause this document to be applied to documents contributed to them
for development, editing, and publication in their respective
Alternate Streams.  If an Alternate Stream manager elects to adopt
this document, they must do so in a manner that is public and
notifies their respective document Contributors that this document
applies to their respective Alternate Streams.  In such case, each
occurrence of the term "Contribution" and "IETF Document" in this
document shall be read to mean a contribution or document in such
Alternate Stream, as the case may be.  It would be advisable for such
Alternate Stream managers to consider adapting the definitions of
"Contribution" and other provisions in this document to suit their

## Rights Contributors Provide to the IETF Trust

In all matters of copyright and document procedures, the intent is to
benefit the Internet community and the public at large, while respecting
the legitimate rights of others.

Under the laws of most countries and current international treaties (for
example the "Berne Convention for the Protection of Literary and
Artistic Work" [Berne]), authors obtain numerous rights in
the works they produce automatically upon producing them.  These rights
include copyrights, moral rights, and other rights.  In many cases, if the
author produces a work within the scope of his or her employment, most
of those rights are usually assigned to the employer, either by
operation of law or, in many cases, under contract.  (The Berne
Convention names some rights as "inalienable", which means that the
author retains them in all cases.)

In order for Contributions to be used within the IETF Standards Process,
including when they are published as Internet-Drafts or RFCs, certain
limited rights must be granted to the IETF Trust, which then grants the
necessary rights to the IETF.  In addition, Contributors must make
representations to the IETF Trust and the IETF regarding their ability
to grant these rights.

### Exposition of Why These Procedures Are the Way They Are

#### Rights Granted in Contributions

The IETF Trust and the IETF must obtain the right to publish an IETF
Contribution as an RFC or an Internet-Draft from the Contributors.

A primary objective of this policy is to obtain from the document authors
only the non-exclusive rights that are needed to develop and publish IETF
Documents and to use IETF Contributions in the IETF Standards Process and
potentially elsewhere.

The authors retain all other rights, but cannot withdraw the above rights
from the IETF Trust and the IETF.

It is important to note that under this document, Contributors are required
to grant certain rights to the IETF Trust (see {{rights-granted}}), which
holds all IETF-related intellectual property on behalf of the IETF community.
The IETF Trust will, in turn, grant a sublicense of these rights to all IETF
participants for use in the IETF Standards Process (see Section 5.4.).  This
sublicense is necessary for the standards development work of the IETF to
continue.  In addition, the IETF Trust may grant certain other sublicenses of
the rights that it is granted under this document.  In granting such other
sublicenses, the IETF Trust will be guided and bound by documents such as
{{RFC5377}}.

#### Rights to Use Contributions

It is important that the IETF receive assurances from all Contributors
that they have the authority to grant the IETF the rights that they
claim to grant because, under the laws of most countries and applicable
international treaties, copyright rights come into existence when a work
of authorship is created (but see {{no-copyright}} regarding public
domain documents), and the IETF cannot make use of IETF Contributions if
it does not have sufficient rights with respect to these copyright
rights.  The IETF and its participants would run a greater risk of
liability to the owners of these rights without this assurance.
To this end, the IETF asks Contributors to give the assurances in
{{rep-and-warranty}}.  These assurances are requested, however, only to the
extent of the Contributor's reasonable and personal knowledge as
defined above.

#### Right to Produce Derivative Works

The IETF needs to be able to evolve IETF Documents in response to experience
gained in the deployment of the technologies described in such IETF
Documents, to incorporate developments in research, and to react to changing
conditions on the Internet and other IP networks.  The IETF may also decide
to permit others to develop derivative works based on Contributions.  In
order to do this, the IETF must be able to produce derivatives of its
documents; thus, the IETF must obtain the right from Contributors to produce
derivative works.  Note that the right to produce translations is required
before any Contribution can be published as an RFC, to ensure the widest
possible distribution of the material in RFCs.  The right to produce
derivative works, in addition to translations, is required for all IETF
Standards Track documents and for most IETF non-Standards Track documents.
There are two exceptions to this requirement: documents describing
proprietary technologies and documents that are republications of the work of
other standards organizations.

The right to produce derivative works must be granted in order for an IETF
working group to accept a Contribution as a working group document or
otherwise work on it.  For non-working group Contributions where the
Contributor requests publication as a Standards Track RFC, the right to
produce derivative works must be granted before the IESG will issue an IETF
Last Call and, for most non-Standards Track, non-working group Contributions,
before the IESG will consider the Internet-Draft for publication.
Occasionally a Contributor may not want to grant publication rights or the
right to produce derivative works before finding out if a Contribution has
been accepted for development in the IETF Standards Process.  In these cases,
the Contributor may include a limitation on the right to make derivative
works in the form specified in the Legend Instructions.  A working group can
discuss the Contribution with the aim to decide if it should become a working
group document, even though the right to produce derivative works or to
publish the Contribution as an RFC has not yet been granted.  However, if the
Contribution is accepted for development, the Contributor must resubmit the
Contribution without the limitation notices before a working group can
formally adopt the Contribution as a working group document.  The IETF Trust
may establish different policies for granting sublicenses with respect to
different types of Contributions and content within Contributions (such as
executable code versus descriptive text or references to third-party
materials).  The IETF Trust's policies concerning the granting of sublicenses
to make derivative works will be guided by {{?RFC5377}}.

The IETF has historically encouraged organizations to publish details of
their technologies, even when the technologies are proprietary, because
understanding how existing technology is being used helps when developing new
technology.  But organizations that publish information about proprietary
technologies are frequently not willing to have the IETF produce revisions of
the technologies and then possibly claim that the IETF version is the "new
version" of the organization's technology.  Organizations that feel this way
can specify that a Contribution be published with the other rights granted
under this document but may withhold the right to produce derivative works
other than translations.

In addition, IETF Documents frequently make normative references to standards
or recommendations developed by other standards organizations.  Since the
publications of some standards organizations are not public documents, it can
be quite helpful to the IETF to republish, with the permission of the other
standards organization, some of these documents as RFCs so that the IETF
community can have open access to them to better understand what they are
referring to.  In these cases, the RFCs can be published without the right
for the IETF to produce derivative works.  In both of the above cases, in
which the production of derivative works is excluded, the Contributor must
include a special legend in the Contribution, as specified in the Legend
Instructions, in order to notify IETF participants about this restriction.

#### Rights to Use Trademarks {#use-trademarks}

Contributors may wish to seek trademark or service mark protection on any
terms that are coined or used in their Contributions.  The IETF makes no
judgment about the validity of any such trademark rights.  However, the IETF
requires each Contributor, under the licenses described in {{rights-granted}}
below, to grant the IETF Trust a perpetual license to use any such trademarks
or service marks solely in exercising rights to reproduce, publish, discuss,
and modify the IETF Contribution.  This license does not authorize the IETF
or others to use any trademark or service mark in connection with any product
or service offering.

#### Contributions Not Subject to Copyright {#no-copyright}

Certain documents, including those produced by the U.S. government and those
which are in the public domain, may not be protected by the same copyright
and other legal rights as other documents.  Nevertheless, we ask each
Contributor to grant to the IETF the same rights he or she would grant, and
to make the same representations, as though the IETF Contribution were
protected by the same legal rights as other documents, and as though the
Contributor could be able to grant these rights.  We ask for these grants and
representations only to the extent that the Contribution may be protected.
We believe they are necessary to protect the
ISOC, the IETF Trust, the IETF,
the IETF Standards Process, and all IETF participants, and because the IETF
does not have the resources or wherewithal to make any independent
investigation as to the actual proprietary status of any document submitted
to it.

#### Copyright in RFCs

As noted above, Contributors to the IETF (or their employers) retain
ownership of the copyright in their Contributions.  This includes
Internet-Drafts and all other Contributions made within the IETF Standards
Process (e.g., via e-mail, oral comment, and otherwise).  However, it is
important that the IETF (through the IETF Trust) own the copyright in
documents that are published as RFCs (other than Informational RFCs and RFCs
that are submitted as RFC Editor Contributions).  Ownership of the copyright
in an RFC does not diminish the Contributors' rights in their underlying
contributions, but it does prevent anyone other than the IETF Trust (and its
licensees) from republishing or modifying an RFC in RFC format.  In this
respect, Contributors are treated the same as anybody else: though they may
extract and republish their own Contributions without limitation, they may
not do so in the RFC format used by the IETF.  And while this principle
(which is included in {{rfc-copyrights}} below) may appear to be new to the
IETF, it actually reflects historical practice and has been observed for many
years through the inclusion of an ISOC or IETF Trust copyright notice on all
RFC documents since the publication of {{?RFC2026}}.

### Rights in Contributions

#### General Policy

By submission of a Contribution, each person actually submitting the
Contribution and each named co-Contributor is deemed to have read and
understood the rules and requirements set forth in this document.  Each
Contributor is deemed, by the act of submitting a Contribution, to enter
into a legally-binding agreement to comply with the terms and conditions
set forth in this document.

The Contributor is further deemed to have agreed that he/she has
obtained the necessary permissions to enter into such an agreement from
any party that the Contributor reasonably and personally knows may have
rights in the Contribution, including, but not limited to, the
Contributor's sponsor or employer.

No further acknowledgment, signature, or other action is required to
bind a Contributor to these terms and conditions.  The operation of the
IETF and the work conducted by its many participants is dependent on
such agreement by each Contributor, and each IETF participant expressly
relies on the agreement of each Contributor to the terms and conditions
set forth in this document.

#### Confidentiality Obligations

No information or document that is subject to any requirement of
confidentiality or any restriction on its dissemination may be submitted
as a Contribution or otherwise considered in any part of the IETF
Standards Process, and there must be no assumption of any
confidentiality obligation with respect to any Contribution.  Each
Contributor agrees that any statement in a Contribution, whether
generated automatically or otherwise, that states or implies that the
Contribution is confidential or subject to any privilege, can be
disregarded for all purposes, and will be of no force or effect.

#### Rights Granted by Contributors to the IETF Trust {#rights-granted}

To the extent that a Contribution or any portion thereof is protected by
copyright or other rights of authorship, the Contributor and each named
co-Contributor grant a perpetual, irrevocable, non-exclusive,
royalty-free, world-wide, sublicensable right and license to the IETF
Trust under all such copyrights and other rights in the Contribution:

1. To copy, publish, display, and distribute the Contribution, in whole
or in part,

2. To prepare translations of the Contribution into languages other
than English, in whole or in part, and to copy, publish, display, and
distribute such translations or portions thereof,

3. To modify or prepare derivative works (in addition to translations)
that are based on or incorporate all or part of the Contribution, and to
copy, publish, display, and distribute such derivative works, or
portions thereof unless explicitly disallowed in the notices contained
in a Contribution (in the form specified by the Legend Instructions),
and

4. To reproduce any trademarks, service marks, or trade names which are
included in the Contribution solely in connection with the reproduction,
distribution, or publication of the Contribution and derivative works
thereof as permitted by this section, provided that when reproducing
Contributions, trademark and service mark identifiers used in the
Contribution, including TM and (R), will be preserved.

#### Sublicenses by the IETF Trust

The IETF Trust will sublicense the rights granted to it under
{{rights-granted}} to all IETF participants for use within the IETF
Standards Process.  This license is expressly granted under a license
agreement issued by the IETF Trust, which can be found at
[Trust Legal Provisions](https://trustee.ietf.org/documents/trust-legal-provisions/).

This license is expressly granted under a license agreement issued by the
IETF Trust and must contain a pointer to the full IETF Trust agreement.

In addition, the IETF Trust may grant additional sublicenses of the licenses
granted to it hereunder.  In doing so, the IETF Trust will comply with the
guidance provided under {{!RFC5377}}.

#### No Patent License

The licenses granted in {{rights-granted}} shall not be deemed to grant any
right under any patent, patent application, or other similar intellectual
property right disclosed by the Contributor under {{sec10}} or
otherwise.

#### Representations and Warranties {#rep-and-warranty}

With respect to each Contribution, each Contributor represents that, to
the best of his or her knowledge and ability:

- The Contribution properly acknowledges all Contributors, including
Indirect Contributors.

- No information in the Contribution is confidential, and the IETF, IETF
Trust, ISOC, and its affiliated organizations may freely disclose any
information in the Contribution.

- There are no limits to the Contributor's ability to make the grants,
acknowledgments, and agreements herein that are reasonably and personally
known to the Contributor.

- The Contributor has not intentionally included in the Contribution
any material that is defamatory or untrue or which is illegal under the
laws of the jurisdiction in which the Contributor has his or her
principal place of business or residence.

- All trademarks, trade names, service marks, and other proprietary
names used in the Contribution that are reasonably and personally known
to the Contributor are clearly designated as such where reasonable.

#### No Duty to Publish

The Contributor, and each named co-Contributor, acknowledges that the
IETF has no duty to publish or otherwise use or disseminate any
Contribution.  The IETF reserves the right to withdraw or cease using any
Contribution that does not comply with the requirements of this section.

#### Trademarks

Contributors who claim trademark rights in terms used in their IETF
Contributions are requested to state specifically what conditions apply
to implementers of the technology relative to the use of such
trademarks.  Such statements should be submitted in the same way as is
done for other intellectual property claims.  (See {{sec5}}.)

#### Copyright in RFCs {#rfc-copyrights}

Subject to each Contributor's (or its sponsor's) ownership of its underlying
Contributions as described in {{rep-and-warranty}} (which ownership is
qualified by the irrevocable licenses granted under {{rights-granted}}), each
Contributor hereby acknowledges that the copyright in any RFC in which such
Contribution is included, other than an RFC that is an RFC Editor
Contribution, shall be owned by the IETF Trust.  Such Contributor shall be
deemed to assign to the IETF Trust such Contributor's copyright interest in
the collective work constituting such RFC upon the submission of such RFC for
publication, and acknowledges that a copyright notice acknowledging the IETF
Trust's ownership of the copyright in such RFC will be included in the
published RFC.

#### Contributors' Retention of Rights

Although Contributors provide specific rights to the IETF, it is not intended
that this should deprive them of their right to exploit their Contributions.
To underscore this principle, the IETF Trust is directed to issue a license
or assurance to Contributors, which confirms that they may each make use of
their Contributions as published in an RFC in any way they wish, subject only
to the restriction that no Contributor has the right to represent any
document as an RFC, or equivalent of an RFC, if it is not a full and complete
copy or translation of the published RFC.

###  Legends, Notices and Other Standardized Text in IETF Documents

The IETF requires that certain standardized text be reproduced verbatim
in certain IETF Documents (including copies, derivative works, and
translations of IETF Documents).  Some of this standardized text may be
mandatory (e.g., copyright notices and disclaimers that must be included
in all RFCs) and some may be optional (e.g., limitations on the right to
make derivative works).  The text itself, as well as the rules that
explain when and how it must be used, is contained in the Legend
Instructions.  The Legend Instructions may be updated from time to time,
and the version of the standardized text that must be included in IETF
Documents is that which was posted in the Legend Instructions on the
date of publication.

The IETF reserves the right to refuse to publish Contributions that do
not include the legends and notices required by the Legend Instructions.

It is important to note that each Contributor grants the IETF Trust
rights pursuant to this document and the policies described herein.  The
legends and notices included in certain written Contributions such as
Internet-Drafts do not themselves convey any rights.  They are simply
included to inform the reader (whether or not part of the IETF) about
certain legal rights and limitations associated with such documents.

It is also important to note that additional copyright notices are not
permitted in IETF Documents except in the case where such document is
the product of a joint development effort between the IETF and another
standards development organization or is a republication of
the work of another standards development organization.  Such exceptions
must be approved on an individual basis by the IAB.

## IPR Disclosures {#ipr-section}

This document refers to the IETF Participant making disclosures,
consistent with the general IETF philosophy that Participants in the
IETF act as individuals.  A Participant's obligation to make a
disclosure is also considered satisfied if the IPR owner, which may
be the Participant's employer or sponsor, makes an appropriate
disclosure in place of the Participant doing so.

### Actions for Documents for Which IPR Disclosure(s) Have Been Received

1. The IESG, IAB, ISOC, and IETF Trust disclaim any responsibility for
identifying the existence of or for evaluating the applicability
of any IPR, disclosed or otherwise, to any IETF technology,
specification, or standard, and will take no position on the
validity or scope of any such IPR.

2. When the IETF Secretariat has received a notification under
{{ipr-voluntary}} of the existence of non-participant IPR that
potentially Covers a technology under discussion at IETF or which
is the subject of an IETF Document, the IETF Secretariat shall
promptly publish such notification and will request that the
identified third party make an IPR disclosure in accordance with
the provisions of {{ipr-section}}.

3. When an IPR disclosure has been made as provided in {{ipr-section}} of
this document, the IETF Secretariat may request from the purported
holder of such IPR a written assurance that upon approval by the
IESG for publication of the relevant IETF specification(s) as one
or more RFCs, all persons will be able to obtain the right to
implement, use, distribute, and exercise other rights with respect
to Implementing Technology under one of the licensing options
specified in {{ipr-licensing}} item 1 below unless a statement identifying
one of the licensing options described in {{ipr-licensing}} item 1 has
already been received by the IETF Secretariat.  The working group
proposing the use of the technology with respect to which the
Intellectual Property Rights are disclosed may assist the IETF
Secretariat in this effort.
The results of this procedure shall not, in themselves, block
publication of an IETF Document or advancement of an IETF Document
along the Standards Track.  A working group may take into
consideration the results of this procedure in evaluating the
technology, and the IESG may defer approval when a delay may
facilitate obtaining such assurances.  The results will, however,
be recorded by the IETF Secretariat and be made available online.

4. The IESG will not make any determination that any terms for the
use of an Implementing Technology (e.g., the assurance of
reasonable and non-discriminatory terms) have been fulfilled in
practice.  It will instead apply the normal requirements for the
advancement of Internet Standards (see {{std-process}}).  If the two
unrelated implementations of the specification that are required
to advance from Proposed Standard to Internet Standard have been produced
by different organizations or individuals, or if the "significant
implementation and successful operational experience" required to
advance from Proposed Standard to Internet Standard has been achieved, the
IESG will presume that the terms are reasonable and to some degree
non-discriminatory.  Note that this also applies to the case where
multiple implementers have concluded that no licensing is
required.
This presumption may be challenged at any time, including during
the Last Call period by sending email to the IESG.

### Who Must Make an IPR Disclosure? {#ipr-who}

#### A Contributor's IPR in His or Her Contribution {#ipr-contrib}

Any Contributor who reasonably and personally knows of IPR meeting
the conditions of {{ipr-level}} which the Contributor believes Covers
or may ultimately Cover his or her written Contribution that is
intended to be used as an input into the IETF Standards Process, or
which the Contributor reasonably and personally knows his or her
employer or sponsor may assert against Implementing Technologies
based on such written Contribution, must make a disclosure in
accordance with {{ipr-section}}.

#### An IETF Participant's IPR in Contributions by Others {#ipr-others}

If an individual's Participation relates to a written Contribution
made by somebody else that is intended to be used as an input into
the IETF Standards Process, and such Participant reasonably and
personally knows of IPR meeting the conditions of {{ipr-level}} which
the Participant believes Covers or may ultimately Cover that
Contribution, or which the Participant reasonably and personally
knows his or her employer or sponsor may assert against Implementing
Technologies based on such written Contribution, then such
Participant must make a disclosure in accordance with {{ipr-section}}.

#### Voluntary IPR Disclosures {#ipr-voluntary}

If any person has information about IPR that may Cover a technology
relevant to the IETF Standards Process, but such person is not
required to disclose such IPR under {{ipr-contrib}} or {{ipr-others}} above,
such person is nevertheless encouraged to file an IPR disclosure as
described in {{ipr-how}} below.  Such an IPR disclosure should be
filed as soon as reasonably possible after the person realizes that
such IPR may Cover a Contribution.  Situations in which such voluntary
IPR disclosures may be made include when (a) IPR does not meet the
criteria in {{ipr-level}} because it is not owned or controlled by an
IETF Participant or his or her sponsor or employer (referred to as
third party IPR), (b) an individual is not required to disclose
IPR meeting the requirements of {{ipr-level}} because that individual is
not Participating in the relevant IETF activity, or (c) the IPR
Covers technology that does not yet meet the criteria for a Contribution
hereunder (e.g., it is disclosed in an informal or other non-IETF
setting).

### The Timing of Disclosure

Timely IPR disclosure is important because working groups need to
have as much information as they can while they are evaluating
alternative solutions.

#### Timing of Disclosure under {{ipr-contrib}}

The IPR disclosure required pursuant to {{ipr-contrib}} must be made
as soon as reasonably possible after the Contribution is submitted
or made unless the required disclosure is already on file.  See
{{ipr-updates}} for a discussion of when updates need to be made for
an existing disclosure.

If a Contributor first learns of IPR in its Contribution that
meets the conditions of {{ipr-level}}, for example a new patent
application or the discovery of a relevant patent in a patent
portfolio, after the Contribution is published in an Internet-
Draft, a disclosure must be made as soon as reasonably possible
after the IPR becomes reasonably and personally known to the
Contributor.

#### Timing of Disclosure under {{ipr-others}}

The IPR disclosure required pursuant to {{ipr-others}} must be made as
soon as reasonably possible after the Contribution is made, unless
the required disclosure is already on file.

Participants who realize that IPR meeting the conditions of
{{ipr-level}} may Cover technology that will be or has been incorporated into a
Contribution, or is seriously being discussed in a working group, are
strongly encouraged to make a preliminary IPR disclosure.  That IPR
disclosure should be made as soon after coming to the realization as
reasonably possible, not waiting until the Contribution is actually
made.

If an IETF Participant first learns of IPR that meets the conditions
of {{ipr-level}} that may Cover a Contribution by another party, for
example a new patent application or the discovery of a relevant
patent in a patent portfolio, after the Contribution is made, an IPR
disclosure must be made as soon as reasonably possible after the
Contribution or IPR becomes reasonably and personally known to the
Participant.

#### Timing of Disclosure by ADs and Others

By the nature of their office, IETF Area Directors or persons
assisting them may become aware of Contributions late in the process
(for example at IETF Last Call or during IESG review) and, therefore
in such cases, cannot reasonably be expected to disclose IPR
Covering those Contributions until they become aware of them.

### How Must an IPR Disclosure be Made? {#ipr-how}

IPR disclosures must be made by following the instructions at
<https://www.ietf.org/ipr-instructions>.  IPR disclosures and other
IPR-related information, including licensing information, must not be
included in RFCs or other IETF Contributions.  The RFC Editor will
remove any IPR-related information from Contributions prior to
publication as an RFC.

### What Must Be in an IPR Disclosure?

#### Content of IPR Disclosures

An IPR disclosure must include the following information to the
extent reasonably available to the discloser: (a) the numbers of any
issued patents or published patent applications (or indicate that the
disclosure is based on unpublished patent applications), (b) the
name(s) of the inventor(s) (with respect to issued patents and
published patent applications), (c) the specific IETF Document(s) or
activity affected, and (d) if the IETF Document is an Internet-Draft,
its specific version number.  In addition, if it is not reasonably
apparent which part of an IETF Document is allegedly Covered by
disclosed IPR, then it is helpful if the discloser identifies the
sections of the IETF Document that are allegedly Covered by such
disclosed IPR.

#### Updating IPR Disclosures {#ipr-updates}

Those who disclose IPR should be aware that as Internet-Drafts
evolve, text may be added or removed, and it is recommended that they
keep this in mind when composing text for disclosures.

1. Unless sufficient information to identify the issued patent was
disclosed when the patent application was disclosed, an IPR
disclosure must be updated or a new disclosure made promptly after
any of the following has occurred: (1) the publication of a
previously unpublished patent application, (2) the abandonment of
a patent application, (3) the issuance of a patent on a previously
disclosed patent application, or (4) a material change to the IETF
Document covered by the Disclosure that causes the Disclosure to
be covered by additional IPR.  If the patent application was
abandoned, then the new IPR disclosure must explicitly withdraw
any earlier IPR disclosures based on the application.  IPR
disclosures against a particular Contribution are assumed to be
inherited by revisions of the Contribution and by any RFCs that
are published from the Contribution unless the disclosure has been
updated or withdrawn.

2. If an IPR holder files patent applications in additional countries
which refer to, and the claims of which are substantially
identical to, the claims of a patent or patent application
previously disclosed in an IPR disclosure, the IPR holder is not
required to make a new or updated IPR disclosure as a result of
filing such applications or the issuance of patents on such
applications.

3. New or revised IPR disclosures may be made voluntarily at any
other time, provided that licensing information may only be
updated in accordance with {{ipr-licensing}} item 3.

4. Any person may submit an update to an existing IPR disclosure.
If such update is submitted by a person other than the submitter
of the original IPR disclosure (as identified by name and email
address), then the IETF Secretariat shall attempt to contact the
original submitter to verify the update.  If the original
submitter responds that the proposed update is valid, the
Secretariat will update the IPR disclosure accordingly.  If the
original submitter responds that the proposed update is not valid,
the IETF Secretariat will not update the IPR disclosure.  If the
original submitter fails to respond after the IETF Secretariat has
made three separate inquiries and at least 30 days have elapsed
since the initial inquiry was made, then the IETF Secretariat will
inform the submitter of the proposed update that the update was
not validated and that the updater must produce legally
sufficient evidence that the submitter (or his/her employer) owns
or has the legal right to exercise control over the IPR subject to
the IPR disclosure.  If such evidence is satisfactory to the IETF
Secretariat, after consultation with the IETF legal counsel, then
the IETF Secretariat will make the requested update.  If such
evidence is not satisfactory, then the IETF Secretariat will not
make the requested update.

#### Blanket IPR Statements {#sec543}

The requirement to make an IPR disclosure is not satisfied by the
submission of a blanket statement that IPR may exist on every
Contribution or a general category of Contributions.  This is the
case because the aim of the disclosure requirement is to provide
information about specific IPR against specific technology under
discussion in the IETF.  The requirement is also not satisfied by a
blanket statement of willingness or commitment to license all
potential IPR Covering such technology under fair, reasonable, and
non-discriminatory terms for the same reason.  However, the
requirement for an IPR disclosure is satisfied by a blanket statement
of the IPR discloser's commitment to license all of its IPR meeting
the requirements of {{ipr-level}} (and either {{ipr-contrib}} or {{ipr-others}})
to implementers of an IETF specification on a royalty-free (and
otherwise reasonable and non-discriminatory) basis as long as any
other terms and conditions are disclosed in the IPR disclosure.

### Licensing Information in an IPR Disclosure {#ipr-licensing}

1. Since IPR disclosures will be used by IETF working groups during
their evaluation of alternative technical solutions, it is helpful
if an IPR disclosure includes information about licensing of the
IPR in case Implementing Technologies require a license.
Specifically, it is helpful to indicate whether, upon approval by
the IESG for publication as an RFC of the relevant IETF
specification(s), all persons will be able to obtain the right to
implement, use, distribute, and exercise other rights with respect
to an Implementing Technology a) under a royalty-free and
otherwise reasonable and non-discriminatory license, or b) under a
license that contains reasonable and non-discriminatory terms and
conditions, including a reasonable royalty or other payment, or c)
without the need to obtain a license from the IPR holder (e.g., a
covenant not to sue with or without defensive suspension, as
described in {{alts}}).

2. The inclusion of a licensing declaration is not mandatory, but it
is encouraged so that the working groups will have as much
information as they can during their deliberations.  If the
inclusion of a licensing declaration in an IPR disclosure would
significantly delay its submission, then the discloser may submit
an IPR disclosure without a licensing declaration and then submit
a new IPR disclosure when the licensing declaration becomes
available.  IPR disclosures that voluntarily provide text that
includes licensing information, comments, notes, or URLs for other
information may also voluntarily include details regarding
specific licensing terms that the IPR holder intends to offer to
implementers of Implementing Technologies, including maximum
royalties.

3. It is likely that IETF will rely on licensing declarations and
other information that may be contained in an IPR disclosure and
that implementers will make technical, legal, and commercial
decisions on the basis of such commitments and information.  Thus,
when licensing declarations and other information, comments,
notes, or URLs for further information are contained in an IPR
disclosure, the persons making such disclosure agree and
acknowledge that the commitments and information contained in such
disclosure shall be irrevocable and will attach, to the extent
permissible by law, to the associated IPR, and all implementers of
Implementing Technologies will be justified and entitled to rely
on such materials in relating to such IPR, whether or not such IPR
is subsequently transferred to a third party by the IPR holder
making the commitment or providing the information.  IPR holders
making IPR disclosures that contain licensing declarations or
providing such information, comments, notes, or URLs for further
information must ensure that such commitments are binding on any
transferee of the relevant IPR, and that such transferee will use
reasonable efforts to ensure that such commitments are binding on
a subsequent transferee of the relevant IPR, and so on.

4. Licensing declarations must be made by people who are authorized
to make such declarations as discussed in {{ipr-level}} of this
document.

### Level of Control over IPR Requiring Disclosure {#ipr-level}

IPR disclosures under {{ipr-contrib}} and {{ipr-others}} are required with
respect to IPR (a) that is owned, directly or indirectly, by the
individual Contributor or his/her employer or sponsor (if any), or (b)
that such persons otherwise have the right to license or assert, or
(c) from which such persons derive a direct or indirect pecuniary
benefit, or (d) as to which an individual Contributor is listed as an
inventor on the relevant patent or patent application.

### Disclosures for Oral Contributions

If a Contribution is oral and is not followed promptly by a written
disclosure of the same material, and if such oral Contribution would
be subject to a requirement that an IPR Disclosure be made (had such
oral Contribution been written), then the Contributor must accompany
such oral Contribution with an oral declaration that he/she is aware
of relevant IPR in as much detail as reasonably possible or file an
IPR Declaration with respect to such oral Contribution that otherwise
complies with the provisions of {{ipr-who}} through {{ipr-level}} above.

### General Disclosures {#general-disclosures}

As described in {{ipr-how}}, the IETF will make available a public
facility (e.g., a web page and associated database) for the posting
of IPR disclosures conforming with the disclosure requirements of
this policy.  In addition, the IETF may make available a public
facility for the posting of other IPR-related information and
disclosures that do not satisfy the requirements of this policy but
which may otherwise be informative and relevant to the IETF ("General
Disclosures").  Such General Disclosures may include, among other
things, "blanket disclosures" that do not contain a royalty-free
licensing commitment as described in {{sec543}}, disclosures of
IPR that do not identify the specific IETF Documents Covered by the
disclosed IPR, and licensing statements or commitments that are
applicable generally and not to specific IPR disclosures.  All of
this information may be helpful to the IETF community, and its
disclosure is encouraged.  However, General Disclosures do not
satisfy an IETF Participant's obligation to make IPR disclosures as
required by this policy.

In some cases, if an IPR disclosure submitted by an IETF Participant
does not meet the requirements of this policy, the IETF may elect to
post the non-conforming IPR disclosure as a General Disclosure in
order to provide the greatest amount of information to the IETF
community.  This action does not excuse the IETF Participant from
submitting a new IPR disclosure that conforms with the requirements
of {{ipr-who}} through {{ipr-level}}.  The IETF reserves the right
to decline to
publish General Disclosures that are not relevant to IETF activities,
that are, or are suspected of being, defamatory, false, misleading,
in violation of privacy or other applicable laws or regulations, or
that are in a format that is not suitable for posting on the IETF
facility that has been designated for General Disclosures.

### Failure to Disclose

There may be cases in which individuals are not permitted by their
employers or by other factors to disclose the existence or substance
of patent applications or other IPR.  Since disclosure is required
for anyone making a Contribution or Participating in IETF activities,
a person who is not willing or able to disclose IPR for this reason,
or any other reason, must not contribute to or participate in IETF
activities with respect to technologies that he or she reasonably and
personally knows may be Covered by IPR which he or she will not
disclose, unless that person knows that his or her employer or
sponsor will make the required disclosures on his or her behalf.

Contributing to or Participating in IETF activities about a
technology without making required IPR disclosures is a violation of
IETF policy.

In addition to any remedies or defenses that may be available to
implementers and others under the law with respect to such a
violation (e.g., rendering the relevant IPR unenforceable), sanctions
are available through the normal IETF processes for handling
disruptions to IETF work.  See {{?RFC6701}} for details regarding the
sanctions defined in various existing Best Current Practice
documents.

### Evaluating Alternative Technologies in IETF Working Groups {#alts}

In general, IETF working groups prefer technologies with no known IPR
claims or, for technologies with claims against them, an offer of
royalty-free licensing.  However, to solve a given technical problem,
IETF working groups have the discretion to adopt a technology as to
which IPR claims have been made if they feel that this technology is
superior enough to alternatives with fewer IPR claims or free
licensing to outweigh the potential cost of the licenses.  To assist
these working groups, it is helpful for the IPR claimants to declare,
in their IPR Declarations, the terms, if any, on which they are
willing to license their IPR Covering the relevant IETF Documents.

1. When adopting new technologies, the participants in an IETF
working group are expected to evaluate all the relevant tradeoffs
from their perspective.  Most of the time these considerations are
based purely on technical excellence, but IPR considerations may also
affect the evaluation and specific licensing terms may affect the
participants' opinion on the desirability of adopting a particular
technology.

2. The IETF has no official preference among different licensing
terms beyond what was stated at the beginning of this section.
However, for information and to assist participants in understanding
what license conditions may imply, what follows are some general
observations about some common types of conditions.  The following
paragraphs are provided for information only:

3. When there is no commitment to license patents covering the
technology, this creates uncertainty that obviously is concerning.
These concerns do not exist when there is a commitment to license,
but the license terms can still differ greatly.  Some common
conditions include 1) terms that are fair, reasonable, and non-
discriminatory, and which may bear royalties or other financial
obligations (FRAND or
RAND); 2) royalty-free terms that are otherwise fair,
reasonable, and non-discriminatory (RAND-z); and 3) commitments
not to assert declared IPR, possibly conditional on reciprocity.  Open
source projects, for instance, often prefer the latter two.  Note that
licenses often come with complex terms that have to be evaluated in
detail, and this crude classification may not be sufficient to make a
proper evaluation.  For instance, licenses may also include
reciprocity and defensive suspension requirements that require
careful evaluation.

4. The level of use of a technology against which IPR is disclosed is
also an important factor in weighing IPR encumbrances and associated
licensing conditions against technical merits.  For example, if
technologies are being considered for a mandatory-to-implement change
to a widely deployed protocol, the hurdle should be very high for
encumbered technologies, whereas a similar hurdle for a new protocol
could conceivably be lower.

5. IETF working groups and IETF areas may, however, adopt stricter
requirements in specific cases.  For instance, the IETF Security Area
has adopted stricter requirements for some security technologies.  It
has become common to have a mandatory-to-implement security
technology in IETF technology specifications.  This is to ensure that
there will be at least one common security technology present in all
implementations of such a specification that can be used in all
cases.  This does not limit the specification from including other
security technologies, the use of which could be negotiated between
implementations.  An IETF consensus has developed that no mandatory-to-implement security technology can be specified in an IETF
specification unless it has no known IPR claims against it or a
royalty-free license is available to implementers of the
specification.  It is possible to specify such a technology in
violation of this principle if there is a very good reason to do so
and if that reason is documented and agreed to through IETF
consensus.  This limitation does not extend to other security
technologies in the same specification if they are not listed as
mandatory to implement.

6. It should also be noted that the absence of IPR disclosures at any
given time is not the same thing as the knowledge that there will be
no IPR disclosure in the future, or that no IPR Covers the relevant
technology.  People or organizations not currently involved in the
IETF or people or organizations that discover IPR they feel to be
relevant in their patent portfolios can make IPR disclosures at any
time.

7. It should be noted that the validity and enforceability of any IPR
may be challenged for legitimate reasons outside the IETF.  The mere
existence of an IPR disclosure should not be taken to mean that the
disclosed IPR is valid or enforceable or actually Covers a particular
Contribution.  Although the IETF can make no actual determination of
validity, enforceability, or applicability of any particular IPR, it
is reasonable that individuals in a working group or the IESG will
take into account their own views of the validity, enforceability, or
applicability of IPR in their evaluation of alternative technologies.

### Change Control for Technologies

The IETF must have change control over the technology described in
any Standards Track IETF Documents in order to fix problems that may
be discovered or to produce other derivative works.

In some cases, the developer of patented or otherwise controlled
technology may decide to hand over to the IETF the right to evolve
the technology (a.k.a., "change control").  The implementation of an
agreement between the IETF and the developer of the technology can be
complex.  (See {{?RFC1790}} and {{?RFC2339}} for examples.)

Note that there is no inherent prohibition against a Standards Track
IETF Document making a normative reference to proprietary technology.
For example, a number of IETF standards support proprietary
cryptographic transforms.

### Licensing Requirements to Advance Standards Track IETF Documents

{{sec611}} states:

> If the technology required to implement the specification
> requires patented or otherwise controlled technology, then
> the set of implementations must demonstrate at least two
> independent, separate and successful uses of the licensing
> process.

A key word in this text is "requires".  The mere
existence of disclosed IPR does not necessarily mean that licenses
are actually required in order to implement the technology.

### No IPR Disclosures in IETF Documents

IETF Documents must not contain any mention of specific IPR.  All
specific IPR disclosures must be submitted as described in {{ipr-section}}.
Readers should always refer to the online web page <https://www.ietf.org/ipr/>
to get a full list of IPR disclosures received by the IETF concerning any
Contribution.

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
Updates (not obsoletes) RFC5378, RFC5657, and RFC7475.

--- back

# Acknowledgments
{:numbered="false"}

We gratefully acknowledge those who have contributed to the development of
IETF RFC's and the processes that create both the content and documents.  In
particular, we thank the authors of all the documents that updated
{{RFC2026}}.

We also thank Sandy Ginoza of the Secretariat for sending all the
original RFC sources.
