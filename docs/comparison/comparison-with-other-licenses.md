# Comparison with other licenses

Reference material for readers who already know the lineage rule in
[the evolution idea](../evolution.md). OSEL 0.1 is not MIT, Apache-2.0,
GPL-3.0, AGPL-3.0, EUPL-1.2, or MPL-2.0.
This page says what it takes from each, and what it does not take. It is
background for the draft. It is not legal advice, and it is not a
compatibility determination. Determinations, including the absence of any
positive one, are in
[known-compatible-licenses.md](../compatibility/known-compatible-licenses.md).

## At a glance

| | OSEL 0.1 | MIT | Apache-2.0 | GPL-3.0 | AGPL-3.0 | EUPL-1.2 | MPL-2.0 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Baseline | Permissive | Permissive | Permissive | Strong copyleft | Strong copyleft, plus network use | Copyleft, with outbound list | File-level copyleft |
| Patent grant | Yes, Section 3 | No | Yes | Yes, Section 11 | Yes, via GPL-3.0 | Limited wording | Yes |
| Patent retaliation | Yes, Section 3.2 | No | Yes | Termination is tied to the whole license | Same as GPL-3.0 | Yes | Yes |
| Downstream license change | Optional, one way, criteria in Section 1.7 | Not a named procedure | Not a named procedure | Same terms required | Same terms required | Named appendix | Named secondary licenses |
| Source disclosure duty | No, unless the replacement target has one | No | No | Yes | Yes, including network use | Yes | Yes, for covered files |
| OSI-approved | No; not submitted | Yes | Yes | Yes | Yes | Yes | Yes |

## MIT

Shared: a short permissive copyright grant, a notice condition, a warranty
disclaimer, and a liability limit. Section 5.3(b) says OSEL is modeled on MIT.

Not shared: MIT has no patent grant, no contributor agreement, and no
replacement procedure. MIT code is often carried into GPL works because the
MIT grant is broad and the notice is kept. That practice depends on the
copyright holders' grant and on GPL's rules about additional terms. OSEL tries
to write the "may move to a stricter license" half of that practice into the
license, and to forbid the "may move to an even thinner license" half when
the move is called a replacement.

The Section 2(e) sublicense sentence is the piece that still reads like MIT.
If it is left unqualified, it may undo the half OSEL is trying to forbid.
See [open question 3](../open-questions.md).

## Apache-2.0

Shared: an express patent license limited to claims tied to the contribution,
and termination of that patent license if the licensee brings patent
litigation.

Apache-2.0 Section 3 licenses patent claims necessarily infringed by a
contribution alone or by combination of the contribution with the work.
OSEL Section 3.1 uses that limiting idea and also says the license covers
derivative works. The drafting notes treat the limitation as borrowed
structure, not as a claim that the two grants have the same claim chart.

Not shared:

- Apache-2.0 requires a NOTICE file to be handled in a stated way, and
  requires modified files to carry a notice of the change. OSEL's baseline
  only requires the copyright and license notices.
- Apache-2.0 includes a trademark sentence. OSEL puts trademark limits in the
  category list for targets, and does not itself grant or fully regulate
  trademarks. The repository license file refuses trademark rights in the
  name OSEL except for nominative use.
- Apache-2.0 has no Section 5 replacement right.
- Apache-2.0 Section 5's contributor representation is narrower than OSEL
  Section 4.1(c).

Apache-2.0 code can be included in a GPLv3 work, on the Free Software
Foundation's published compatibility view, and cannot be included in a
GPLv2-only work. That is a fact about Apache and the GPL. It is not a fact
about whether Apache-2.0 is a Compatible License under OSEL Section 1.7.

## GPL-3.0

Shared: a concern that downstream recipients keep patent coverage, and a
concern that a distributor not add further restrictions that take the work
private. OSEL expresses the second concern only after a recipient elects a
stricter license. GPL-3.0 expresses it as the default.

Not shared: GPL-3.0 requires derivatives to be conveyed under GPL-3.0 and
requires corresponding source. OSEL requires neither until a replacement
succeeds. GPL-3.0 is not "MIT plus a patent clause." OSEL is closer to that
description, with the replacement option added.

Section 3 was influenced by GPL-3.0 Section 11 and does not copy it.
Section 11's essential-patent-claim definition excludes claims infringed only
as a consequence of further modification. Section 3.1's combination language
is the Apache pattern. Section 3.4's election exists because the drafters did
not want replacement to be read as cancelling the patent grant, and they also
saw that a target such as GPL-3.0 brings its own patent section. The election
is an open issue, not a completed bridge. See the
[drafting notes](../rationale/drafting-notes.md).

GPL-3.0 Section 7 is cited at the end of OSEL Section 1.7. That citation does
not match Section 7's list. The comparison worth keeping is thematic:
both texts try to allow a small set of extra notice, name, and marking terms,
and both try to refuse other added restrictions. OSEL's category (ii) goes
past GPL Section 7, because copyleft itself is the extra requirement OSEL is
willing to accept as a target.

## AGPL-3.0

AGPL-3.0 is GPL-3.0 plus a duty to offer source to users who interact with
the program over a network. OSEL has no network clause. A replacement with
AGPL-3.0 would add one, if AGPL-3.0 were a Compatible License.

The draft's reading of that duty, for Section 5.3(c), is that it regulates
disclosure. It does not forbid offering the software as a service. OSD
criterion 6, which AGPL-3.0 has already passed in its own approval, uses
"used in a business" as an example of a field that must not be forbidden.
Nothing in this paragraph decides the Section 1.7(b) question for AGPL-3.0.

## EUPL-1.2

Shared idea: a downstream distributor may, in a defined case, distribute a
work under another selected license, while the earlier licensing history is
not erased.

The mechanisms differ.

- EUPL-1.2 is copyleft. OSEL 0.1 is permissive unless replaced.
- EUPL-1.2 names compatible licenses in an appendix. The Official Journal
  text includes GPL-2.0, GPL-3.0, AGPL-3.0, LGPL-2.1, LGPL-3.0, MPL-2.0,
  OSL-2.1, OSL-3.0, EPL-1.0, CeCILL-2.0, CeCILL-2.1, LiLiQ-R, LiLiQ-R+,
  EUPL-1.1, EUPL-1.2, and CC-BY-SA-3.0 for works other than software. The
  European Commission may update that appendix to later versions of those
  licenses under stated conditions.
- OSEL 0.1 names no target. It points at OSI approval plus Section 1.7.
- EUPL-1.2 includes choice of law and forum. OSEL 0.1 includes neither.
- EUPL's compatibility clause is about interoperability of a copyleft work
  with other copyleft works. OSEL's replacement right is about moving a
  permissive work toward a stricter OSI license.

The EUPL design is the main existence proof that "outbound compatibility"
can be written as part of an OSI-approved license. It is also the main
existence proof that a named list is a workable alternative to an open-ended
test. OSEL's choice of the open-ended test is intentional in 0.1, and it is
the choice most likely to be re-examined. See
[open question 11](../open-questions.md).

## MPL-2.0

Shared idea: a specifically described downstream licensing permission, not a
general right to invent a new license.

MPL-2.0's copyleft stops at the file boundary. Its Section 3.3 secondary
licenses are GPL-2.0, LGPL-2.1, AGPL-3.0, and later versions of those,
unless the covered software is marked incompatible with secondary licenses.
The recipient of MPL code does not apply a "stricter than MPL" test. The
license either names the secondary license or it does not.

OSEL does not adopt file-level copyleft, an exhibit of license names, or an
incompatible-secondary-licenses marker. A project that wants "MPL, unless we
opt out of GPL compatibility" already has MPL-2.0. OSEL's different bet is a
permissive default with a criteria-based ratchet. That bet is unfinished
while the criteria are not operational.

## What OSEL is not trying to be

- A badge of OSI approval. The draft has not been submitted.
- A way to add a noncommercial, ethical, or business-model restriction and
  still call the result open source. Section 5.3(c) forbids that target, and
  the OSD forbids that license.
- A delayed-release or source-available license. There is no change date after
  which a proprietary grant becomes OSEL. Rights under Section 2 exist from
  the grant.
- A contributor license agreement standing beside the license. Section 4 is
  inside the license. Projects that need assignment, a developer certificate
  of origin, or a jurisdiction-specific CLA still need those instruments.
  Section 4 does not replace them for every project policy.

## Choosing among them, in practical terms

Use a license that already exists if its terms are the terms you want.

- Choose MIT or BSD when you want a short permissive grant and you accept the
  absence of a patent clause.
- Choose Apache-2.0 when you want that patent clause and the NOTICE practice,
  without a relicensing procedure.
- Choose GPL-3.0 or AGPL-3.0 when share-alike, or network share-alike, is the
  rule from the first release.
- Choose MPL-2.0 when you want file-level share-alike and a named GPL
  secondary path.
- Choose EUPL-1.2 when you want copyleft, a named outbound list, and the
  EUPL's own legal frame.
- OSEL 0.1 is a draft for the remaining case: permissive now, with an express
  and limited power for a later distributor to assume a stricter OSI license.
  That case is the draft's only reason to exist. The text is not stable
  enough to recommend as the license for a production project that needs a
  predictable obligation set.
