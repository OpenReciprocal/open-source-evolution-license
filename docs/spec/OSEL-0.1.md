# Annotated specification: OSEL Version 0.1

This page reads the published 0.1 text. The idea, and the discussion draft
that restates it as a Menu, are in
[docs/evolution.md](../evolution.md) and
[`LICENSES/OSEL-0.2-draft.txt`](../../LICENSES/OSEL-0.2-draft.txt).

This page is a reading guide. The operative text is
[`LICENSES/OSEL-0.1.txt`](../../LICENSES/OSEL-0.1.txt). If this page and that
file disagree, the plain-text file controls.

OSEL 0.1 is a working draft. It is not OSI-approved. This guide is not legal
advice.

## What the draft is trying to do

OSEL starts from a permissive grant, close to MIT, and adds three mechanisms:

1. A bounded patent license, with retaliation termination (Section 3).
2. A contributor grant, so a submission can be maintained and relicensed
   under the replacement rule without a later signature (Section 4).
3. A one-way replacement right. On distribution of a new version, a recipient
   may move that version to a stricter OSI-approved Compatible License
   (Section 5). The recipient may also keep OSEL.

The direction is deliberate. Replacement may add obligations inside a closed
list of categories. It may not drop obligations, and it may not add field-of-use
or user restrictions.

## How a distribution can lawfully leave the maintainer

```text
Receive software under OSEL 0.1
        |
        +-- Distribute that version under OSEL 0.1
        |     (notices preserved; patent grant passed through)
        |
        +-- Distribute a new version under a Compatible License
              only if every Section 5.1 condition is met
              and the target is not excluded by Section 5.3
```

There is no third path written on purpose. Whether Section 2(e) accidentally
opens one is [open question 3](../open-questions.md).

Versions already distributed stay under OSEL (Section 5.1(d)). The replacing
recipient must keep the OSEL text and the original copyright notices with the
replaced version (Section 5.1(e)).

## Section 1, definitions

Section 1.1 pins this draft to Version 0.1. There is no "or any later version"
clause. Software released under 0.1 does not move to a later draft by itself.

Section 1.2 defines Software broadly: source, object, documentation, and
related files. The replacement right follows that whole work, not a single
source file, unless a later draft says otherwise.

Section 1.3 defines Contributor by intentional submission for inclusion.
Communication marked "Not a Contribution" is excluded. Oral communication can
count. That is wide, and projects that adopt the draft will want a written
contribution channel.

Section 1.4 defines Recipient as anyone who obtains a copy under this license,
including people who never contribute.

Section 1.5 defines OSI-Approved License by OSI certification and listing,
and then repeats that the license must meet all ten OSD criteria. The second
sentence lets a reader reopen an OSI decision. See
[open question 11](../open-questions.md).

Section 1.6 defines Replacement as the Section 5 act. It says the new license
applies to "subsequent versions." Section 5.1(d) is more precise: the named
version and versions after it. Read them together. Earlier versions are not
rewritten.

Section 1.7 is the compatibility gate. It is analyzed in
[criteria.md](../compatibility/criteria.md). Three conditions are cumulative:
OSI approval without added restrictions, a stricter obligation set, and a
closed list of what the extra requirements may be about.

## Section 2, basic grant

The copyright grant covers use, reproduction, modification, distribution, and
sublicensing. It is royalty-free and not limited by field, user, or manner of
use. The non-discrimination sentences are there to track OSD criteria 5 and 6.

The only condition on the copyright grant is notice preservation: the
copyright notice and this license notice stay with copies and substantial
portions. That is the MIT-style baseline Section 5.3(b) refers to when it
says OSEL is modeled on MIT.

"Irrevocable" is not defined. Section 8 still terminates rights for an
uncured breach. See [open question 6](../open-questions.md).

The grant is phrased as a grant by "the Copyright Holder," a term Section 1
does not define. See [open question 4](../open-questions.md).

## Section 3, patent grant

Section 3.1 is a per-contributor and per-copyright-holder patent license.
It covers making, using, selling, offering for sale, importing, and otherwise
exploiting the Software and derivative works. The claims covered are only
those owned or controlled by that grantor and necessarily infringed by the
contribution alone, or by the combination of the contribution with the
Software. The point, stated in the original drafting notes, is to avoid a
grant over patents that have no substantial relation to the contribution.
Apache-2.0 Section 3 uses the same limiting idea.

Section 3.2 ends that patent license if the recipient, including its
Affiliates, starts patent litigation alleging that the Software or a
Contribution infringes a patent. A cross-claim or counterclaim counts.
Non-patent claims do not. "Affiliates" is undefined.

Section 3.3 is a distributor duty: pass this patent grant through, and do not
impose stricter patent restrictions on the next recipient.

Section 3.4 says replacement does not by itself end or shrink the Section 3.1
grant. The recipient may elect an equivalent or stronger patent license in
the target. Section 3.2 always remains for the original contributor's grant.
The election is the main patent open issue. See
[open question 5](../open-questions.md) and the
[drafting notes](../rationale/drafting-notes.md).

Section 3.5 separates the patent license from the copyright license. A
copyright breach does not void the patent license, except for Section 3.2.
A recipient who loses copyright rights under Section 8 may still hold the
patent license. That is generous to the recipient. It is a design choice of
this draft, not an OSD requirement.

## Section 4, contributor grant

Section 4.1 attaches when a contributor submits work for inclusion, unless
the submission is marked "Not a Contribution." The contributor:

- grants copyright rights to maintainers and all recipients;
- accepts that the contribution is under OSEL from submission, and waives
  conflicting assertions;
- confirms authority, and confirms non-infringement of third-party
  intellectual property.

The non-infringement confirmation is broader than Apache-2.0 Section 5. See
[open question 7](../open-questions.md).

Section 4.2 is the advance consent that makes replacement possible in a
multi-author project. Contributors authorize any recipient to exercise
Section 5 without asking again. The authorization starts when the
contribution is included, and it travels with further distribution.

Section 4.3 keeps copyright with the contributor. OSEL is a license, not an
assignment.

## Section 5, replacement

Section 5.1 gives every recipient the replacement right at the moment of
distribution. All of the following are required:

| Condition | What it requires |
| --- | --- |
| 5.1(a) | An actual distribution. A declaration with no distribution does nothing. |
| 5.1(b) | The target is a Compatible License under Section 1.7. |
| 5.1(c) | A `LICENSE-REPLACEMENT.md` file in the root directory, with the four listed items. |
| 5.1(d) | No effect on versions distributed before the replacement. |
| 5.1(e) | The OSEL text and the original copyright notices stay in the tree. |

The statement required by Section 5.1(c)(i) has a fixed shape. The example
is [`examples/LICENSE-REPLACEMENT.md`](../../examples/LICENSE-REPLACEMENT.md).
That example is a form. It is not a finding that any named license is compatible.

Section 5.2 locks the replacing recipient in. That recipient cannot ship the
replaced version again under OSEL or under a less restrictive license. Other
people who still have an earlier OSEL copy are not locked. They never
exercised the right.

Section 5.3 states three prohibitions: no non-OSI license, no license with
equal or fewer obligations (MIT and BSD are the examples), and no license
that adds field-of-use, user, or business-model restrictions. The third
prohibition is the draft's answer to OSD criteria 5 and 6.

"Business models" is wider than the OSD's own examples. A license can add a
source-disclosure duty for network use without forbidding a business. That
kind of duty is aimed at Section 1.7(c)(ii), not at Section 5.3(c). The
distinction matters for AGPL-3.0, and it is not decided. See the
[working list](../compatibility/known-compatible-licenses.md).

Section 5.4 is the succession rule. Target terms govern the replaced version.
Three things survive anyway:

- notices and attribution, at the stricter of the two licenses;
- Sections 6 and 7, unless the target's disclaimer and liability limit are
  equivalent or stronger;
- Section 3, unless Section 3.4's election applies.

## Sections 6 and 7, disclaimer and liability

Section 6 disclaims warranties, including merchantability, fitness for a
particular purpose, and noninfringement, and then adds a short liability
limit. Section 7 repeats the liability limit in the longer MIT/BSD form.
See [open question 10](../open-questions.md).

These sections are written in capitals, following the convention of the
MIT text. Capitalization does not decide enforceability. Some jurisdictions
limit how far a disclaimer can go. Section 9.1, severability, is the draft's
response if a court cuts one sentence down.

## Section 8, termination

An uncured breach automatically ends the recipient's rights. Cure within 30
days after the first written notice restores them automatically. Who can give
that notice is not specified.

Section 8.2 confirms that after a valid replacement, OSEL no longer governs
that recipient's later distribution of the replaced line, except for the
Section 5.4 survivors.

## Section 9, general

Severability, no waiver, and an entire-agreement clause. The entire-agreement
clause needs an exception for a valid replacement. See
[open question 9](../open-questions.md).

## Instructions after the license text

The block titled "Instructions for Applying This License" sits after the line
"(End of License Text)." It tells a project to put a short notice at the top
of each source file and to keep the full text in a `LICENSE` file. Those
instructions are part of the published draft file. They are application
guidance for downstream projects. A worked copy of the notice is in
[`examples/source-header.txt`](../../examples/source-header.txt).

## Terms that do not appear, on purpose or by omission

The draft does not:

- require disclosure of source, unless and until a replacement license does;
- name a choice of law or venue;
- grant trademark rights;
- contain an "or later version" upgrade;
- list Compatible Licenses by name;
- state that it is OSI-approved.

The missing definitions in [open question 4](../open-questions.md) are
omissions, not policy.
