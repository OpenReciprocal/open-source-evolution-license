# Open Source Evolution License (OSEL)

Any recipient may ship a copy under a stricter OSI-approved license drawn
from a fixed menu of duties. Those stricter terms stick to that copy and to
copies made from it. No one may ship that sticky copy under a weaker
license. No other copy is rewritten.

The maintainer does not own the future of the line. The future also cannot
run backward.

That sentence is the license. Read it in
[docs/evolution.md](docs/evolution.md), or in
[中文](docs/translations/zh-CN-idea.md).
Patent language, contributor language, and the notice file exist to keep the
sentence true.

## Two drafts

| | What it is |
| --- | --- |
| [LICENSES/OSEL-0.1.txt](LICENSES/OSEL-0.1.txt) | Published working draft of 2026-09-26. The step is called Replacement. The compatibility test is not yet one a reader can apply. |
| [LICENSES/OSEL-0.2-draft.txt](LICENSES/OSEL-0.2-draft.txt) | Discussion draft. The step is called Evolution. The test is the Evolution Menu. It does not amend 0.1. |

Neither draft has been submitted to the Open Source Initiative. Neither is
an OSI-approved license. Do not describe either as "OSI Approved" or
"OSI Certified."

Software released under 0.1 stays under 0.1. There is no "or any later
version" clause. Choosing the 0.2 discussion draft means putting that file
in `LICENSE`, on purpose.

## Status

The names "Open Source Evolution License" and "OSEL" identify these drafts.
A project that needs a license other people already know how to apply should
use an OSI-approved license. The non-operative notes that once sat at the
bottom of the 0.1 file are in
[docs/rationale/drafting-notes.md](docs/rationale/drafting-notes.md).

## The Menu

A descendant may take on added duties of five kinds only: attribution,
source disclosure (including share-alike), patents, names and trademarks,
and marks of what changed. A noncommercial limit, an ethical-use ban, or a
thinner permissive license is not on the Menu. The step happens by shipping
a modified version with a record. It does not happen by announcement.

In 0.1 the record is `LICENSE-REPLACEMENT.md` and the test is Section 1.7.
That test does not yet determine that any particular license passes. MIT and
BSD are excluded by name. In the 0.2 discussion draft the record is
`EVOLUTION.md` and the test is Section 1.11. The draft still does not
pre-approve a named target. The recipient maps the target onto the Menu
before shipping.

Conserved across a step: the use of the software in any field, the patent
promise already made (neither shrunk nor rewritten onto someone else), the
papers of the ancestor, and the ancestor version itself.

## Key documents

Start with the idea, then the draft that tries to close it.

| Document | What it is |
| --- | --- |
| [docs/evolution.md](docs/evolution.md) | The idea, the Menu, and three scenes. |
| [docs/translations/zh-CN-idea.md](docs/translations/zh-CN-idea.md) | The same idea in Simplified Chinese. |
| [LICENSES/OSEL-0.2-draft.txt](LICENSES/OSEL-0.2-draft.txt) | Discussion draft in which the Menu is operative. |
| [LICENSES/OSEL-0.2-draft.md](LICENSES/OSEL-0.2-draft.md) | Reading map for that draft. |
| [examples/EVOLUTION.md](examples/EVOLUTION.md) | Form of the 0.2 record. |
| [LICENSES/OSEL-0.1.txt](LICENSES/OSEL-0.1.txt) | Published 0.1 text. |
| [docs/spec/OSEL-0.1.md](docs/spec/OSEL-0.1.md) | Annotated reading of 0.1. |
| [docs/open-questions.md](docs/open-questions.md) | What 0.1 left open, and what 0.2-draft answers. |
| [docs/compliance/osd-checklist.md](docs/compliance/osd-checklist.md) | 0.1 against the Open Source Definition. Not a legal opinion. |
| [docs/compatibility/criteria.md](docs/compatibility/criteria.md) | How to read 0.1 Section 1.7. |
| [docs/comparison/comparison-with-other-licenses.md](docs/comparison/comparison-with-other-licenses.md) | Reference, when the job is a different job. |

The full index is [docs/README.md](docs/README.md). Project upkeep lives in
[CONTRIBUTING.md](CONTRIBUTING.md), [GOVERNANCE.md](GOVERNANCE.md),
[ROADMAP.md](ROADMAP.md), and [FAQ.md](FAQ.md).

## How to apply a draft

To apply Version 0.1, put [LICENSES/OSEL-0.1.txt](LICENSES/OSEL-0.1.txt) in a
file named `LICENSE`. The copyright notice is `Copyright (c) 2026 OpenReciprocal`. To apply the 0.2
discussion draft, use [LICENSES/OSEL-0.2-draft.txt](LICENSES/OSEL-0.2-draft.txt)
the same way. Do not mix the two records: 0.1 uses
`LICENSE-REPLACEMENT.md`; the 0.2 draft uses `EVOLUTION.md`.

### Version 0.1

Add this notice at the top of each source file. A copy with a suggested
SPDX identifier is in [examples/source-header.txt](examples/source-header.txt).

```text
Copyright (c) 2026 OpenReciprocal

This software is released under the Open Source Evolution License
(OSEL), Version 0.1. That license permits Recipients, subject to
specified conditions, to evolve the license into an OSI-Approved
Compatible License that imposes additional obligations. The complete
license text is available in the LICENSE file in the project root
directory.
```

`LicenseRef-OSEL-0.1` is a project-local SPDX identifier. OSEL is not on the
SPDX License List.

If you distribute a new version and exercise Section 5, create
`LICENSE-REPLACEMENT.md` in the root of the software. It must contain the
items required by Section 5.1(c). The file in
[examples/LICENSE-REPLACEMENT.md](examples/LICENSE-REPLACEMENT.md) shows the
form. Filling in a target license is a compatibility conclusion. Version 0.1
does not supply that conclusion.

### Version 0.2 discussion draft

Use the notice printed at the end of
[LICENSES/OSEL-0.2-draft.txt](LICENSES/OSEL-0.2-draft.txt). A step under that
draft is a shipped modified version plus
[examples/EVOLUTION.md](examples/EVOLUTION.md). The draft does not name a
license that already passes the Menu. The recipient does that mapping, or
does not take the step.

## Compliance and the Open Source Definition

OSEL is designed to be consistent with the Open Source Definition. The most
frequently discussed issue is whether the replacement right in Section 5
conflicts with OSD criterion 3.

OSD criterion 3 states that a license must allow modifications and derived
works to be distributed under the same terms as the license of the original
software. It does not require that a license must require distribution under
the same terms. The word "allow" is not the same as "require."

OSEL preserves the recipient's ability to distribute derivative works under
OSEL itself. Section 2(d) grants the right to distribute the software and
derivative works. The replacement right in Section 5 is an additional option.
It does not remove the option to use OSEL.

The replacement right is intended to expand the freedoms available to
recipients. Section 5.2 makes one recipient's election stick for the replaced
version. That stickiness is a review flag, discussed in the
[OSD checklist](docs/compliance/osd-checklist.md). This repository does not
treat it as settled by the paragraph above.

The other frequent questions concern OSD criteria 5 and 6, which prohibit
discrimination against persons, groups, and fields of endeavor. OSEL addresses
those criteria through Section 1.7(c), which limits additional obligations to
a closed list of categories, and through Section 5.3(c), which prohibits
replacement with a license that adds restrictions on field of use, users, or
business models.

The checklist is a draft analysis, not a legal opinion.

## Relationship to other licenses

OSEL shares with MIT a permissive baseline. It adds a patent grant, a
contributor grant, and the replacement mechanism in Section 5.

OSEL shares with Apache-2.0 a patent grant and patent retaliation
termination. The patent grant in Section 3.1 is limited to patent claims that
are necessarily infringed by the contribution itself or by the combination of
the contribution with the software.

OSEL shares with EUPL-1.2 and MPL-2.0 the idea that a downstream recipient
may, under stated conditions, distribute a new version under another license.
Unlike those two, OSEL 0.1 does not use a fixed list. Section 1.7 anchors
compatibility in OSI approval and in the categories in Section 1.7(c).

That difference is intentional. It is also one of the issues likely to draw
scrutiny if OSEL is submitted for certification. The longer comparison is
[docs/comparison/comparison-with-other-licenses.md](docs/comparison/comparison-with-other-licenses.md).

## Contributing

Contributions to the specification are welcome. Read
[CONTRIBUTING.md](CONTRIBUTING.md) first.

In summary:

1. Open an issue before a substantial change to the license text.
2. Use the issue templates.
3. Keep the change focused, and explain the reason.
4. Be ready to discuss the Open Source Definition.
5. Contributions to the license text are offered under CC0-1.0 so they can be
   merged into the public-domain license text. Documentation contributions
   are under CC-BY-4.0 unless you mark them otherwise.

## Frequently asked questions

The longer list is [FAQ.md](FAQ.md).

**Is OSEL an OSI-approved license?**
No. Version 0.1 has not been submitted.

**Can I use OSEL for my project now?**
You may use the draft text. Review it first. Later versions may change it.
A project that needs a stable license should use an OSI-approved license.

**Does the replacement right violate OSD criterion 3?**
The draft's position is that it does not, because distribution under OSEL
remains allowed. The sticky election in Section 5.2 is an open review flag.
See the [checklist](docs/compliance/osd-checklist.md).

**Can a recipient replace OSEL with MIT or BSD?**
No. Section 5.3(b) prohibits a license with fewer or equal obligations.

**Can a recipient replace OSEL with GPL-3.0?**
GPL-3.0 is OSI-approved and imposes additional obligations. Whether it is a
Compatible License is open. See
[known-compatible-licenses.md](docs/compatibility/known-compatible-licenses.md).

**Does replacement affect the patent license?**
Section 3.4 says the Section 3.1 patent license does not end or shrink merely
because of replacement. Section 3.2 continues to apply. If the target
provides an equivalent or stronger patent license, the recipient may elect
that target's patent provisions. Whether the election can enlarge an original
contributor's grant is an [open question](docs/open-questions.md).

**Is any of this legal advice?**
No. For a commercial or high-risk use, consult a qualified lawyer.

## Repository layout

```text
README.md
LICENSE
LICENSES/
    OSEL-0.1.txt
    OSEL-0.1.md
    OSEL-0.2-draft.txt
    OSEL-0.2-draft.md
docs/
    evolution.md
    spec/OSEL-0.1.md
    rationale/
    compliance/
    compatibility/
    comparison/
    translations/zh-CN-idea.md
    translations/zh-CN.md
examples/
    EVOLUTION.md
    LICENSE-REPLACEMENT.md
    source-header.txt
```

## Roadmap

The live text is the 0.2 discussion draft. Comment on the Menu, on
share-alike as a Menu duty, and on the failed-step rule. A catalog of
license names is a different instrument, and this draft does not adopt one.
Details are in [ROADMAP.md](ROADMAP.md).

## License of this repository

The OSEL license text is dedicated to the public domain under CC0-1.0.

The documentation, drafting notes, translations, and other non-license
materials are licensed under CC-BY-4.0 unless a file says otherwise.

See [LICENSE](LICENSE).

This repository does not grant trademark rights in "Open Source Evolution
License" or "OSEL" beyond nominative use.

## Disclaimer

Both drafts may contain errors, ambiguities, or provisions that are not
enforceable in some jurisdictions. Neither has been reviewed by the Open
Source Initiative or by any court.

Nothing in this repository constitutes legal advice. Use at your own risk.
