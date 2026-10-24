# Frequently asked questions

Short answers. The license text you applied wins if an answer and that text
disagree. These answers are not legal advice. The idea is stated in
[docs/evolution.md](docs/evolution.md).

## The idea

### What is OSEL for?

A line of software that starts permissive, whose descendants may take on
more duties from a fixed menu, and whose ancestors stay as they were shipped.
The maintainer does not keep a private power to relicense, and no recipient
gains a power to make the line thinner.

### Which file do I apply?

Version 0.1 if you want the published draft, knowing its compatibility test
does not yet yield a "yes" for ordinary licenses. The 0.2 discussion draft
if you want the Menu as the operative test. They are different licenses.
One project should put one of them in `LICENSE`.

### Does evolution happen by itself?

No. Someone has to ship a modified version with a valid record. A project
can live its whole life under OSEL and never take the step.

## Status

### Is OSEL an OSI-approved license?

No. Version 0.1 is a working draft. It has not been submitted to the Open
Source Initiative. Do not call it OSI-approved or OSI-certified.

### Can I use OSEL for a project now?

You can apply the draft if you have reviewed it and you can live with later
versions saying something else. Software already released under 0.1 stays
under 0.1 unless its copyright holders relicense it. There is no "or any
later version" clause.

A project that needs a license other people already understand should use an
OSI-approved license. The [comparison](docs/comparison/comparison-with-other-licenses.md)
suggests which existing license is closer to several common goals.

### Is this repository legal advice?

No. It has not been reviewed by OSI or by a court. For a commercial or
high-risk deployment, ask a qualified lawyer.

### Which file is the license?

[`LICENSES/OSEL-0.1.txt`](LICENSES/OSEL-0.1.txt) is canonical.
[`LICENSES/OSEL-0.1.md`](LICENSES/OSEL-0.1.md) is the same text with Markdown
headings. Drafting notes are not part of the license.

### Which language controls?

English. The [Simplified Chinese translation](docs/translations/zh-CN.md) is
there so readers can follow the structure. It is not a second official text.

## What the license allows

### Does OSEL require me to publish source code?

Not by itself. The baseline is permissive. A replacement target may require
source disclosure. That duty appears only if someone validly exercises
Section 5 and the target actually contains it.

### Can I sell the software, or use it in a product, or offer it as a service?

Section 2 grants use for any purpose and distribution without a field limit.
OSEL does not forbid sale or a service. A later replacement license might add
a source duty. Section 5.3(c) forbids a replacement that adds a restriction
on a field of use, a class of users, or a business model.

### Does OSEL grant trademark rights?

No. The repository statement in [LICENSE](LICENSE) also withholds trademark
rights in the name "OSEL," except nominative use to identify the draft.

### Do contributors keep their copyright?

Yes. Section 4.3 says the grants are not an assignment.

### Can a contributor opt out of a single submission?

Yes. Mark that communication in writing as "Not a Contribution." Section 1.3
and Section 4.1 then exclude it. The rest of an unmarked submission is covered.

### Does "irrevocable" mean the license cannot end?

It is not defined. The intended reading is that the licensor cannot revoke at
will. Section 8 still ends rights for an uncured breach. Section 3.2 still
ends the patent license if the recipient starts the patent litigation
described there. See [open question 6](docs/open-questions.md).

## Replacement

### Does every downstream user have to leave OSEL?

No. Replacement is optional and happens only when a recipient distributes a
new version and satisfies Section 5.1. Anyone can keep distributing under
OSEL.

### Can a recipient replace OSEL with MIT or BSD?

No. Section 5.3(b) prohibits a target with fewer or equal obligations, and it
names MIT and BSD.

### Can a recipient replace OSEL with GPL-3.0 or AGPL-3.0?

The draft does not decide. Both are OSI-approved and stricter in the everyday
sense. Section 1.7(b)'s strict-superset test is not settled, and the patent
interaction is an open issue. The working list records them as "not
determined."

### Can a recipient add a noncommercial or ethical-use restriction?

No. That kind of rider is not the OSI-approved license it modifies, and
Section 5.3(c) forbids restrictions on users, fields, or business models.

### What has to be in LICENSE-REPLACEMENT.md?

Four things, from Section 5.1(c):

1. The replacement statement, in the form the license quotes.
2. The full text of the target license, or a link to the official text.
3. A short explanation of which Section 1.7(c) categories the extra
   requirements fall into.
4. The name or identifier of the recipient who is exercising the right.

The notice is required at the time of distribution. A declaration that does
not accompany a distribution does nothing (Section 5.1(a)).

### Does replacement rewrite older releases?

No. Section 5.1(d) limits it to the version named in the notice and to
subsequent versions. Older distributions remain under OSEL.

### Can the replacing recipient change their mind?

Not for that replaced version. Section 5.2 says the replacement binds that
recipient's later distribution of it. They may not ship that version under
OSEL or under a less restrictive license. Other people who hold a pre-replacement
copy are not bound by someone else's election.

### Does the patent license survive replacement?

Section 3.4 says it does not end or shrink merely because of the replacement.
Section 3.2's retaliation rule continues for the original contributor's grant.
The recipient may elect the target's patent provisions if they are equivalent
or stronger. Whether that election can put new patent duties on the original
contributor is open. See the [drafting notes](docs/rationale/drafting-notes.md).

## Using the draft in a tree

### What identifier should a scanner see?

A reasonable project-local identifier is `LicenseRef-OSEL-0.1`. OSEL is not
an SPDX-listed license. Do not write `SPDX-License-Identifier: MIT` on
OSEL code.

### How do I apply it?

Put the full text in `LICENSE`, fill in the copyright line, and add the
per-file notice from [examples/source-header.txt](examples/source-header.txt).

### Can I dual-license?

The draft does not discuss dual licensing. A copyright holder can offer
their own code under more than one license. In a multi-author project,
Section 4 covers contributions submitted for inclusion under OSEL. It is not
a grant to dual-license other people's contributions under an unrelated
second license. Get advice before you promise a dual license.

### What if my package has no root directory?

Section 5.1(c) currently requires `LICENSE-REPLACEMENT.md` in the root
directory. A distribution that cannot hold that file has no conforming
replacement procedure in version 0.1. Shipping under OSEL does not need the
file. A later draft may allow an equivalent notice. See
[open question 8](docs/open-questions.md).

## The document set

### May I copy the license text into my project?

Yes. The license text is under CC0-1.0 so that adoption is possible. See
[LICENSE](LICENSE).

### May I translate or fork the documentation?

The handbook is under CC-BY-4.0. Keep attribution, and do not present a
modified draft as OSEL 0.1. If you change operative wording, use a different
name or a different version.

### Who maintains this repository?

The OpenReciprocal project. Decision rules are in
[GOVERNANCE.md](GOVERNANCE.md). The initial 0.1 text was committed by
lemonhub-io.
