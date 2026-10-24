# Open questions in OSEL 0.1

This list collects issues that the 0.1 text does not settle. The discussion
draft at [`LICENSES/OSEL-0.2-draft.txt`](../LICENSES/OSEL-0.2-draft.txt)
answers them by replacing the strict-superset test with the Evolution Menu.
That draft is not an amendment of 0.1. This list is not legal advice.

Suggested directions, still non-operative, are in
[proposed clarifications for 0.2](rationale/proposed-0.2.md).

## 1. The Compatible License test is not yet operational

Section 1.7(b) says two things at once:

- the target imposes obligations that are more numerous or more specific; and
- the target's set of obligations strictly contains OSEL's set.

License obligations are not nested sets. A copyleft license adds source and
share-alike duties, and it also withdraws the permissive sublicense that
Section 2(e) grants. "More obligations" and "strict superset" can therefore
give different answers for the same license.

Until that test is restated, or replaced by a fixed list, this repository
does not treat any license as a determined Compatible License. MIT and the
BSD family are excluded by Section 5.3(b). Everything stricter remains
unresolved. See [known-compatible-licenses.md](compatibility/known-compatible-licenses.md).

## 2. The citation to GPLv3 Section 7 does not match the list

The last sentence of Section 1.7 says the categories "refer to the enumerated
list of acceptable additional terms in Section 7(b) of GPLv3."

GPLv3 Section 7's additional-terms list is subsections (a) through (f), not
subsection (b) alone. Those subsections cover warranty disclaimers,
attribution, marking modified versions, publicity limits on names, trademark
declinations, and indemnification. They do not include copyleft source
disclosure or a patent grant. OSEL categories (ii) and (iii) are therefore
outside the GPL list, and GPL items (a) and (f) are outside the OSEL list.

The cross-reference needs to be rewritten or removed.

## 3. Section 2(e) can be read as a path around Section 5

Section 2(e) lets a recipient sublicense the Section 2 rights for modified
versions. Section 5.3(b) forbids replacement with MIT or BSD. A reader can
argue that a sublicense under MIT is not a "replacement" and is therefore
still allowed.

If that reading stands, the one-way ratchet does not work. A later draft
should say whether a sublicense must keep OSEL's conditions, or must itself
be under OSEL or a Compatible License.

## 4. Several terms used in operative sections are undefined

The text uses these terms without defining them:

- Project
- Project maintainers
- Copyright Holder
- Contribution, as a noun (Section 1.3 defines Contributor and Submit)
- Affiliates (Section 3.2)
- Target License (Sections 3.4 and 5.4)
- Original License (the replacement statement in Section 5.1(c)(i))

"Copyright Holder" is especially important. Section 2 reads as one grant by
"the Copyright Holder." Apache-2.0 is explicit that each contributor licenses
only its own contribution. OSEL should be equally explicit, so that one
contributor is not read as licensing another contributor's work or patents.

## 5. Section 3.4 may be read as enlarging the original patent grant

Section 3.4 lets a recipient elect the target license's patent provisions
when they are "equivalent or stronger." The drafting note in the original
0.1 file already asks whether that election can place patent duties on the
original contributor that the contributor did not accept.

A safer reading is that the election changes which patent terms the
electing recipient passes downstream, and does not widen the grant the
original contributor already made. The text does not say that clearly.
Section 3.2's retaliation clause is stated to survive either way.

## 6. "Irrevocable" sits next to termination

Section 2 and Section 3.1 describe the grants as irrevocable. Section 8.1
terminates rights on breach, with a 30-day cure. Section 3.2 terminates the
patent license if the recipient starts patent litigation.

The usual reading of "irrevocable" in this kind of grant is that the licensor
cannot take it back at will. Termination for breach or for patent aggression
is a different event. The draft should say so.

## 7. Section 4.1(c) is broader than a typical contributor representation

The contributor confirms authority to grant the licenses, and also confirms
that the contribution "does not infringe any third party's intellectual
property rights." Apache-2.0 Section 5 requires authority and that the
submission is an original work or is submitted with sufficient rights. It
does not require a general non-infringement warranty.

The broader sentence will surprise contributors. A later draft should say
whether it is intentional.

## 8. The replacement notice assumes a filesystem

Section 5.1(c) requires a file named `LICENSE-REPLACEMENT.md` in "the root
directory of the Software." That fits a source tree. It is awkward for a
single-file distribution, a firmware image, a package format, or a network
service that has no root directory.

Open Source Definition criterion 10 says no provision may be predicated on
any individual technology or style of interface. The basic grant in Section 2
is technology-neutral. The replacement procedure is not. A later draft can
accept an equally prominent notice when the medium has no root directory.

## 9. Section 9.3 can collide with a valid replacement

Section 9.3 says this license is the entire agreement and supersedes prior
agreements. After a valid replacement, Section 5.4 says the target license
applies, with listed OSEL provisions surviving. Those two sections need an
express order of precedence.

## 10. Sections 6 and 7 overlap

Section 6 is a warranty disclaimer and, in its second sentence, a short
limitation of liability. Section 7 is a longer limitation of liability. The
overlap is not fatal, and it is a common pattern, but the two formulations
are not identical. A later draft can make Section 6 the disclaimer only.

## 11. OSI approval is a moving compatibility oracle

Section 1.7 depends on the OSI approved list as it stands at the time of
replacement, together with a private check that the license still meets the
OSD. That has three consequences:

- a license approved years from now can become a candidate without a new
  OSEL version;
- a recipient, or a court, may be asked to decide what OSI had approved and
  whether that license really meets all ten OSD criteria;
- OSEL gives an outside body a role in the meaning of OSEL.

EUPL-1.2 and MPL-2.0 avoid this by naming the downstream licenses. A fixed
list is easier to apply and easier to review. It also goes stale unless a
new OSEL version can add names. Version 0.1 deliberately chose the open
anchor. Whether to keep it is a design choice, not a settled conclusion.

## 12. What "obligations of this License" includes

A recipient who distributes under OSEL, and does not replace it, has a small
set of duties: keep the copyright and license notices (Section 2), pass
through the patent grant, and not tighten patent restrictions (Section 3.3).
Contributor statements in Section 4 bind contributors, not every distributor.
Section 5 duties apply only to someone who chooses replacement.

The strict-superset test is sensitive to which of these count. The draft
does not say.

## 13. No delivery rule for the cure notice

Section 8.1 restores rights if the breach is cured within 30 days after "the
first written notice." It does not say who may give notice, or what counts
as receipt. That matters once more than one copyright holder exists.
