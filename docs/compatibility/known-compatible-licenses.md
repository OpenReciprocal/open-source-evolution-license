# Working list: possible Compatible Licenses

Version 0.1 does not determine that any license is a Compatible License.

This list applies [criteria.md](criteria.md) far enough to separate licenses
the text itself excludes from licenses that stay unresolved. It is
provisional. It will change if Section 1.7 changes. It is not legal advice
and not an OSI position.

Status values used here:

| Status | Meaning |
| --- | --- |
| Excluded | Section 5.3 or Section 1.7(a) rejects it on the facts stated. |
| Not determined | It may be stricter and OSI-approved, and the Section 1.7(b) test still does not yield a yes. |
| Out of scope | It is not a software-license candidate under this draft. |

No row uses "compatible" as a status.

## Excluded

| License | Why it is excluded |
| --- | --- |
| MIT | Section 5.3(b). Fewer obligations than OSEL. The draft names this example. |
| BSD-2-Clause, BSD-3-Clause | Section 5.3(b). The draft names BSD. Attribution and name clauses in BSD-3-Clause do not make it stricter than OSEL's notice, patent, and contributor terms. |
| ISC, 0BSD | Fewer or equal obligations. Section 5.3(b). |
| Unlicense, CC0-1.0 used as the software license | Not a stricter obligation set. CC0 is also not the tool this draft uses for software. |
| A modified GPL, Apache, or MPL with an added restriction | Section 1.7(a) and Section 5.3(a). The modification is a different license and is not OSI-approved as modified. |
| Commons Clause, Business Source License, or another source-available rider | Not an OSI-approved license. Also fails Section 5.3(c) when it restricts a business model. |
| Server Side Public License (SSPL) | Not an OSI-approved license. |
| A noncommercial exception added to an otherwise approved license | The combination is not the approved text. The exception restricts a field or a business model and fails Section 5.3(c). |
| Ethical-use or nationality restrictions | Fail Section 5.3(c), and they are not OSI-approved in that form. |

## Not determined

These licenses are OSI-approved, in the version named, and they add duties
that at least arguably sit inside Section 1.7(c). They are not listed as
compatible. The strict-superset sentence in Section 1.7(b) is the shared
blocker. Individual rows add further blockers.

| License | Obligations that may fit Section 1.7(c) | Why the result stays open |
| --- | --- | --- |
| Apache-2.0 | NOTICE and attribution (i); patent grant and retaliation (iii); trademark (iv); modified-file notices (v) | The patent formula differs from Section 3.1. Apache has no contributor non-infringement confirmation of the Section 4.1(c) kind. The sets are not nested. Apache is also not "more numerous" in every dimension. |
| MPL-2.0 | File-level source and share-alike (ii); notices (i); patent terms (iii) | File-level copyleft withdraws permissive sublicensing rather than containing it. Secondary-license rules and the patent retaliation clause need a separate reading. Exhibit B software raises a further case. |
| LGPL-2.1, LGPL-3.0 | Library copyleft and source duties (ii); notices (i) | Weaker than GPL, still not a superset of OSEL. LGPL-2.1 has no Apache-style patent grant. |
| GPL-2.0-only and GPL-2.0-or-later | Copyleft and source (ii); change notices (v) | No express patent grant of the Section 3 kind. Replacing might be read as dropping patent terms even though Section 5.4(c) tries to keep Section 3. "Or later" adds GPL-3.0 as a possible further license, which is a separate question. |
| GPL-3.0-only and GPL-3.0-or-later | Copyleft and source (ii); patent license (iii); marking changes (v) | This is the case the FAQ leaves open. GPL-3.0 Section 11 is not the same grant as Section 3.1. Additional restrictions are forbidden by GPL Section 10, which interacts badly with an unclear survival of OSEL terms under Section 5.4. The superset test fails on a formal reading. |
| AGPL-3.0-only and AGPL-3.0-or-later | GPL-3.0 duties plus network source disclosure (ii) | Same open issues as GPL-3.0. The network duty is a source-disclosure rule, not a field ban, so Section 5.3(c) does not by itself exclude it. That classification is a reading, not a determination that AGPL passes Section 1.7(b). |
| EUPL-1.2 | Copyleft, source, and a compatibility appendix (ii); attribution (i) | The appendix is a closed outbound list, which is a different mechanism. EUPL also has choice of law and venue. Those terms are not in Section 1.7(c). Whether they are "additional requirements" that disqualify the license is unanswered. |
| OSL-3.0 | Reciprocal source disclosure (ii) | Reciprocal obligations are in the right neighborhood for category (ii). The rest of the OSL, including its termination and acceptance mechanics, has not been mapped category by category. |
| EPL-1.0, EPL-2.0 | Weak copyleft (ii); patent retaliation (iii) | Some EPL terms allocate indemnity or commercial-contributor duties that may fall outside Section 1.7(c). Not mapped to a yes. |
| CDDL-1.0 | File-level reciprocity (ii); patent terms (iii) | Same class of problem as MPL: stricter in one dimension, differently shaped overall. |
| Artistic-2.0 | Several alternative compliance paths | The alternatives make "the set of obligations" hard to state. Left unresolved on purpose. |

### GPL-3.0, stated carefully

The question "may a recipient replace OSEL 0.1 with GPL-3.0?" has a short
answer: the draft does not decide.

The reasons it is the license people ask about:

- it is OSI-approved;
- it adds source and share-alike duties of the kind Section 1.7(c)(ii) names;
- it has its own patent section, which Section 1.7(c)(iii) contemplates;
- Section 3.4 was written with GPL Section 11 in mind, and the drafting notes
  leave the interaction open.

The reasons it is not listed as compatible:

- its obligations do not strictly contain OSEL's small notice-and-patent set
  while also simply adding more; they replace the permissive remainder;
- Section 5.4 can keep OSEL patent, disclaimer, and notice terms alive beside
  GPL terms, and GPL-3.0 is hostile to further restrictions;
- a recipient who elects GPL patent terms may appear to speak for contributors
  who granted only Section 3.1.

A `LICENSE-REPLACEMENT.md` that names GPL-3.0 anyway would assert a
conclusion this project has not reached. Do not copy the example file into
that assertion.

### EUPL-1.2's own list is not OSEL's list

The Official Journal text of EUPL-1.2, Commission Implementing Decision (EU)
2017/863, lists compatible licenses in its appendix, including GPL-2.0,
GPL-3.0, AGPL-3.0, LGPL-2.1, LGPL-3.0, MPL-2.0, OSL-2.1, OSL-3.0, EPL-1.0,
CeCILL-2.0, CeCILL-2.1, LiLiQ-R, LiLiQ-R+, and CC-BY-SA-3.0 for works other
than software. That appendix answers an EUPL question: which licenses may
receive a derivative of EUPL code.

It does not answer the OSEL question. OSEL compatibility runs in the opposite
direction and uses Section 1.7, not the EUPL appendix. The appendix is cited
here only so the two lists are not confused.

### MPL-2.0 secondary licenses are not OSEL's list

MPL-2.0 Section 3.3 permits a larger work to be distributed under a secondary
license, GNU GPL 2.0, LGPL 2.1, AGPL 3.0, or later versions of those, unless
the MPL software is marked incompatible with secondary licenses. That is a
fixed clause with a fixed set of names. OSEL 0.1 has no equivalent exhibit.
Passing MPL's test is not passing Section 1.7.

## Out of scope

| Item | Why |
| --- | --- |
| CC-BY-4.0, CC-BY-SA-4.0 | Creative Commons does not recommend these for software, and they are not the OSI-approved software licenses this draft is aimed at. CC-BY-SA-3.0 appears in the EUPL appendix for non-software works only. |
| The documentation license of this repository | CC-BY-4.0 covers the handbook. It is not a target for replacing OSEL on software. |
| OSEL 0.1 itself | Replacement means a change to another license. Shipping under OSEL is the default, not a replacement. |
| A later OSEL version | Version 0.1 has no "or later" clause. Moving a 0.1 project to 0.2 requires the copyright holders, or a replacement if 0.2 ever qualifies under Section 1.7, which a later permissive draft might not. |

## How to propose an update to this list

Open an issue with the nine-step pattern in
[criteria.md](criteria.md). A pull request that changes a row from
"not determined" to a positive determination needs an operative change to
Section 1.7, or a versioned compatible-license list adopted as part of the
license. A documentation-only edit cannot create that determination.
