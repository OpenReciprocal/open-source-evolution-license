# OSD checklist for OSEL 0.1

Supporting analysis of the published 0.1 text. The project's own statement
of the mechanism is [the evolution idea](../evolution.md). The 0.2
discussion draft is not what this checklist scores.

This is a draft reading of OSEL Version 0.1 against the Open Source
Definition published by the Open Source Initiative. The criteria quoted
below are the OSD text. The annotations are this project's review notes.

This page is not an OSI decision, not a certification opinion, and not legal
advice. OSEL 0.1 has not been submitted for approval. Do not describe it as
OSI-approved.

The OSD is the definition of open source software's distribution terms. A
license can be written toward those criteria and still fail review, because
review also asks whether the text is clear and whether it is distinct enough
to justify another license. Those process points are at the end.

Official text: <https://opensource.org/osd>

## Summary

| Criterion | Draft position | Residual review flag |
| --- | --- | --- |
| 1. Free redistribution | Met by Section 2, if the target of a replacement is itself OSD-compliant | Low, dependent on the target |
| 2. Source code | Met in the same way MIT is met: source distribution is allowed and not obstructed | Low |
| 3. Derived works | Distribution under OSEL remains allowed; replacement is an option | Medium, because Section 5.2 makes an election sticky |
| 4. Integrity of the author's source | No restriction on distributing modified source | Low |
| 5. No discrimination against persons or groups | Stated in Section 2 and guarded by Sections 1.7(c) and 5.3(c) | Medium, because "users" and "business models" need a stable reading |
| 6. No discrimination against fields of endeavor | Same guards as criterion 5 | Medium |
| 7. Distribution of license | Rights attach on obtaining a copy; no extra signature | Low, with a notice-form issue |
| 8. Not specific to a product | No product-specific grant | Low |
| 9. Must not restrict other software | The OSEL baseline does not bind neighboring programs | Low for the baseline; the target license supplies its own rules |
| 10. Technology-neutral | The grant is neutral; the replacement file name is not | Medium |

"Met" in this table means "the draft is written to satisfy the criterion."
It does not mean OSI has agreed.

## 1. Free redistribution

OSD:

> The license shall not restrict any party from selling or giving away the
> software as a component of an aggregate software distribution containing
> programs from several different sources. The license shall not require a
> royalty or other fee for such sale.

OSEL Section 2 grants distribution and sublicensing, royalty-free, without a
field limit. It does not forbid sale, and it does not forbid shipping the
software beside other programs.

A replacement target has to be an OSI-approved license, which itself has to
meet this criterion. Section 5.3(c) also forbids a target that adds
restrictions on business models. A fee for the license grant would fail both
the OSD and Section 5.3.

Patent retaliation in Section 3.2 is not a royalty. It ends the patent
license of a recipient who sues. Apache-2.0, which is OSI-approved, has a
similar clause. That comparison is an analogy, not a ruling about OSEL.

## 2. Source code

OSD:

> The program must include source code, and must allow distribution in source
> code as well as compiled form. Where some form of a product is not
> distributed with source code, there must be a well-publicized means of
> obtaining the source code for no more than a reasonable reproduction cost,
> preferably downloading via the Internet without charge. The source code must
> be the preferred form in which a programmer would modify the program.
> Deliberately obfuscated source code is not allowed. Intermediate forms such
> as the output of a preprocessor or translator are not allowed.

Section 1.2 includes source code in the Software. Section 2(d) allows
distribution in source or object form. OSEL does not require the distributor
to offer source. MIT does not either, and MIT is OSI-approved. The OSD's
source requirement is satisfied for a permissive license by permitting source
distribution and by not authorizing obfuscation as a substitute for source.
The person who releases a program under OSEL is expected to release the
source, because the program, not only the license text, has to meet criterion
2.

If a recipient replaces OSEL with a copyleft license, that target's source
duties apply to the replaced version under Section 5.4. Those duties are
additional. They are the sort of duty Section 1.7(c)(ii) describes. They do
not relax criterion 2.

## 3. Derived works

OSD:

> The license must allow modifications and derived works, and must allow them
> to be distributed under the same terms as the license of the original
> software.

Section 2(c) allows modification and derivative works. Section 2(d) allows
their distribution. Nothing in Section 5 withdraws the right to distribute a
derivative under OSEL. A recipient who never exercises replacement remains
on OSEL.

The OSD says the license must allow distribution under the same terms. It
does not say the license must require distribution under the same terms.
Copyleft licenses require the same terms and therefore also allow them.
Permissive licenses allow the same terms and also allow other terms. OSEL is
written as the second kind, plus an express procedure for the other terms.

Two features will draw review:

- Section 5.2. After a valid replacement, that recipient cannot put the
  replaced version back under OSEL or under a less restrictive license. The
  draft's position is that the same-terms permission existed and the
  recipient elected not to use it for that version. Reviewers may instead say
  that a license which can become forbidding of the same terms, even by
  election, is in tension with criterion 3. This repository does not treat
  that objection as answered. It treats it as the main criterion 3 flag.
- Section 5.1(d) and (e). Earlier distributions stay under OSEL, and the
  OSEL text stays in the replaced tree. That preserves a same-terms copy of
  the pre-replacement work. It does not, by itself, give downstream
  recipients of only the replaced version a right to ignore the target
  license.

Section 2(e), the sublicense grant, is discussed as a drafting gap in
[open question 3](../open-questions.md). If it allows an MIT sublicense, the
criterion 3 permission is safe and the ratchet is not. If it is read narrowly,
the ratchet is stronger and criterion 3 depends entirely on the continuing
OSEL option. Either reading should be made express before a submission.

## 4. Integrity of the author's source code

OSD:

> The license may restrict source-code from being distributed in modified form
> only if the license allows the distribution of "patch files" with the source
> code for the purpose of modifying the program at build time. The license
> must explicitly permit distribution of software built from modified source
> code. The license may require derived works to carry a different name or
> version number from the original software.

OSEL does not restrict distribution of modified source. Section 2(c) and 2(d)
permit modified works in source and object form. It does not require a name
change. A target license might require marking of modifications. That
requirement is inside Section 1.7(c)(v), and it is a kind of requirement the
OSD itself permits.

The replacement notice identifies the version that moved. It does not rename
the software.

## 5. No discrimination against persons or groups

OSD:

> The license must not discriminate against any person or group of persons.

Section 2 states that the rights are not limited by user and that the license
does not discriminate against any person or group. The grant runs to "any
Recipient obtaining a copy."

The replacement right could undermine that sentence if a target could exclude
a group. Section 1.7(c) does not list exclusion of persons as an allowed extra
requirement. Section 5.3(c) forbids replacement with a license that adds
restrictions on users. A noncommercial rider, an "ethical use" rider, or a
nationality restriction fails Section 5.3(c) and fails this criterion.

The residual flag is interpretive. Section 5.3(c) uses "users" and "business
models" in one list with "field of use." A reviewer will ask whether those
words are criteria 5 and 6 restated, or a new and vaguer limit. The draft's
intended reading is the restatement. The text should say that in a later
version if the project wants the intended reading to be the only one.

## 6. No discrimination against fields of endeavor

OSD:

> The license must not restrict anyone from making use of the program in a
> specific field of endeavor. For example, it may not restrict the program
> from being used in a business, or from being used for genetic research.

Section 2 grants use for any purpose and says the license does not
discriminate against any field of endeavor. Section 5.3(c) forbids a target
that adds field-of-use or business-model restrictions, and it cites criteria
5 and 6.

An additional source-disclosure duty, including a duty that arises when users
interact with the program over a network, is not by itself a ban on a field.
AGPL-3.0 is OSI-approved and contains that kind of duty. Under OSEL, such a
duty has to be justified, if at all, as Section 1.7(c)(ii): scope, timing, or
manner of source disclosure. It is not justified as a field restriction, and
Section 5.3(c) does not need to be read as banning it. The working list leaves
AGPL-3.0 unresolved for other reasons, chiefly the strict-superset test.

A license that allows private use and forbids commercial use is a field
restriction. It is outside Section 1.7(c) and inside Section 5.3(c)'s ban.

## 7. Distribution of license

OSD:

> The rights attached to the program must apply to all to whom the program is
> redistributed without the need for execution of an additional license by
> those parties.

Section 1.4 and Section 2 attach rights to any person who obtains a copy.
They do not ask for a signed license or a click-through. Section 3.3 requires
the patent grant to be passed through.

After replacement, the target license's own terms have to satisfy this
criterion, because the target has to be OSI-approved. Section 5.1(c) requires
the replacement notice to include the target text or a link to it, and
Section 5.1(e) requires the OSEL text to remain. Downstream recipients should
not have to go looking for a separate agreement.

The residual flag is formal. A distribution that cannot hold
`LICENSE-REPLACEMENT.md` may be unable to complete Section 5.1(c), even
though the underlying rights did not depend on that file. That is a defect in
the replacement procedure. See [open question 8](../open-questions.md). It is
also the criterion 10 issue below. It does not, on the draft's reading,
condition the Section 2 grant itself.

## 8. License must not be specific to a product

OSD:

> The rights attached to the program must not depend on the program's being
> part of a particular software distribution. If the program is extracted from
> that distribution and used or distributed within the terms of the program's
> license, all parties to whom the program is redistributed should have the
> same rights as those that are granted in conjunction with the original
> software distribution.

OSEL does not tie the grant to a named product or a named distribution. A
copy taken out of a larger aggregate remains under OSEL, or under the target
license if that copy is part of a version that was validly replaced.

Section 5.1(d) supports this criterion for historical versions: extracting an
older version does not cause it to inherit a later replacement.

## 9. License must not restrict other software

OSD:

> The license must not place restrictions on other software that is
> distributed along with the licensed software. For example, the license must
> not insist that all other programs distributed on the same medium must be
> open-source software.

OSEL does not say that other programs on the same medium must be open source.
Section 2's grant is about the Software and derivative works.

A target copyleft license has its own rule about what is a derivative work
and what is a mere aggregate. That rule is the target's rule. OSEL does not
add an aggregation duty of its own. A reviewer may ask whether Section 5.4
causes target copyleft to be an OSEL restriction on other software. The
draft's answer is no: criterion 9 has always been read so that a copyleft
license may govern derivatives without governing independent programs shipped
beside them. GPL-3.0 is OSI-approved on that reading. The answer holds only
if replacement is itself a permitted election under criterion 3.

## 10. License must be technology-neutral

OSD:

> No provision of the license may be predicated on any individual technology
> or style of interface.

Sections 2 through 4 and 6 through 9 do not depend on a language, an
operating system, or an interface. Section 5.1(c) does depend on a named
filename and a root directory. That is a technology assumption.

The assumption is procedural. A recipient who does not replace the license
never needs the file. A recipient who distributes a form that has no root
directory currently has no conforming way to replace. [Proposal 8](../rationale/proposed-0.2.md)
would keep the filename for ordinary source trees and allow an equivalent
prominent notice otherwise.

This flag is real, and it is fixable without changing the policy of Section 5.

## Other review pressures

OSD compliance is not the only question a certification review would ask.

- Clarity. The undefined terms, the two-part test in Section 1.7(b), and the
  wrong GPLv3 citation are clarity problems. Ambiguity that changes who can
  do what is material. The [open questions](../open-questions.md) are the
  list to close before any submission.
- Distinction. OSEL is a new permissive text with a relicensing procedure.
  License proliferation is a standing concern. The rationale has to explain
  why MIT plus a contributor agreement, or EUPL's appendix, or MPL's
  secondary licenses, do not already do the job. The
  [comparison](../comparison/comparison-with-other-licenses.md) is the start
  of that explanation, not the end of it.
- Standing of the oracle. Using "whatever OSI later approves" inside the
  operative definition asks OSI's list to do work inside someone else's
  license. Some reviewers will want a closed list instead. The project has
  not chosen.

## What this checklist does not claim

It does not claim that OSEL 0.1 would pass a review. It claims that the draft
was written against the ten criteria, that the author's position on criterion
3 is "allow, not require," and that the open flags above are the ones a
serious reading should not skip.
