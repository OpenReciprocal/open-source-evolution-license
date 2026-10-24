# Drafting notes

These notes are non-operative. They explain choices in OSEL Version 0.1.
They do not change the license. The notes that originally sat at the end of
`LICENSES/OSEL-0.1.txt` are preserved here and then expanded.

Nothing on this page is legal advice.

## The permissive baseline

Section 2 is modeled on the MIT grant: use, copy, modify, distribute, and
sublicense, for any purpose, with a notice condition. The draft says this
in Section 5.3(b). The extra material is the patent grant, the contributor
grant, and the replacement right.

The baseline is permissive so that a recipient can always ship a derivative
under OSEL itself. Replacement is an added option. The project's reading of
OSD criterion 3 depends on that option remaining real. See the
[OSD checklist](../compliance/osd-checklist.md).

## Why replacement moves only toward stricter licenses

A permissive license can already be carried into a stricter license in
practice, because the permissive grant allows sublicensing and does not
forbid adding conditions when the copyright holder of the new material agrees.
That practical path is uneven in a multi-author work. Each author may have
granted only the original permissive terms.

OSEL states the path in the license and takes the consent up front
(Section 4.2). The path is one way. A recipient may assume additional
obligations inside Section 1.7(c). A recipient may not use the replacement
right to drop down to MIT or BSD (Section 5.3(b)), and may not add
discrimination by person, field, or business model (Section 5.3(c)).

The one-way shape is the feature that distinguishes OSEL from a plain MIT
license, and also from EUPL-1.2 and MPL-2.0, which name specific downstream
licenses rather than describing a direction of travel.

## Patent grant

The original 0.1 note said:

> This formal draft includes the patent grant in Section 3. It draws
> structurally on the experience of Section 3 of Apache 2.0 and Section 11
> of GPLv3, with two adaptations.
>
> First, the "necessarily infringing" limitation in Section 3.1. Section 3.1
> limits the patent license to patent claims that are necessarily infringed
> by the Contribution itself or by the combination of the Contribution with
> the Software. This is intended to avoid forcing a Contributor to grant a
> patent license for patents that have no substantial relation to its
> Contribution. Apache 2.0 adopts a similar limiting logic.
>
> Second, the interface between the patent license and the replacement right.
> Section 3.4 makes clear that the patent license does not automatically
> terminate upon license replacement. This is necessary because the patent
> license is an independent right granted directly by the Contributor to the
> Recipient, and its effect should not be extinguished by the replacement of
> the license text. However, the retaliation termination provision in
> Section 3.2 is retained to protect Contributors against patent litigation
> threats.

Apache-2.0 Section 3 licenses claims infringed by the contribution alone or
by combination of the contribution with the work to which it was submitted.
GPLv3 Section 11 licenses "essential patent claims" in the contributor
version, and excludes claims that would be infringed only because of further
modification. OSEL 3.1 follows the Apache combination wording, and it extends
the license to derivative works. Those are related formulas. They are not the
same formula. A later draft should not describe them as interchangeable.

Section 3.2 follows the Apache retaliation pattern: patent litigation by the
licensee ends the patent license, and non-patent claims do not. OSEL also
names Affiliates, without defining them, and names the Project as a protected
target of the litigation, without defining Project.

Section 3.5, independence of the patent license from a copyright breach, is
not taken from Apache-2.0 or GPLv3. Under this draft a copyright termination
does not, by itself, end the patent license. Only Section 3.2 does that among
the termination rules. The reason to write it down is the replacement
mechanism: the patent grant should not flicker on and off because the
copyright license text changed. The cost is that a recipient who has breached
the copyright terms may still be a patent licensee. Reviewers should treat
that as an intentional, and debatable, allocation of risk.

## The open patent issue, as stated in the 0.1 draft

The original file left this issue open:

> If the Target Compatible License itself contains stronger patent provisions
> than Section 3 (for example, Section 11 of GPLv3 requires that the patent
> license automatically extend to all downstream recipients without additional
> restrictions), Section 3.4 allows the Recipient to elect to apply the
> patent provisions of the Target License. Whether this could impose patent
> obligations on the original Contributor that it did not agree to needs
> further clarification in a future version. One possible improvement is to
> clarify in Section 3.4 that the patent provisions of the Target License may
> replace this Section only if they provide protection to Recipients no less
> than that provided by Section 3.1, and may not reduce the original
> Contributor's rights under the retaliation termination provision in
> Section 3.2.

Two corrections of emphasis belong next to that note.

First, GPLv3 Section 11 is a contributor grant for that contributor's
essential claims. A downstream distributor does not, merely by relicensing,
gain power to widen some other person's patent grant. OSEL should say this
in the operative text. Section 3.4 currently says the recipient may "elect to
apply the patent provisions of the Target License," which can be misread as
an election that binds the original contributor.

Second, "stronger" is ambiguous. A target provision can be stronger for
recipients (a broader claim set, fewer conditions) and at the same time
heavier for the original contributor. The draft's suggested improvement
protects recipients against a reduction and protects contributors against
loss of retaliation. It does not yet say that the election cannot enlarge
the original grant. [Proposal 5](proposed-0.2.md) would add that sentence.

Section 3.3 still matters after any election. A distributor must pass the
patent grant through and must not add stricter patent restrictions. If the
election is used, the draft should say which grant is being passed through.

## Contributor consent in advance

Without Section 4.2, replacement in a project with more than one copyright
holder is a relicensing problem. Each holder would have to agree. Section 4.2
takes that agreement at submission time and makes it run with the
distribution.

The agreement is limited to replacement with a Compatible License. It is not
a blank grant to pick any license. The limit is only as good as the
definition of Compatible License. That definition is the largest open drafting
problem. See [open question 1](../open-questions.md).

Section 4.3 keeps ownership with the contributor so that OSEL is not read as
an assignment to the project.

## Why the notice file exists

Section 5.1(a) refuses a replacement that is only a declaration. Something
has to be distributed. Section 5.1(c) then requires a named file so that a
recipient can see who replaced the license, which version moved, which
license it moved to, and which Section 1.7(c) categories are claimed.

The file name and the "root directory" wording are more specific than they
need to be. The goal is a prominent, durable notice. [Proposal 8](proposed-0.2.md)
would allow an equivalent notice when the distribution has no root directory.

## What the categories are for

Section 1.7(c) is a closed list so that "stricter" cannot mean "stricter in
any way a drafter invents." Extra duties have to be about notices, source
disclosure, patents, trademarks or names, or identification of changes.

The list is the draft's main safeguard for OSD criteria 5 and 6, together
with the express ban in Section 5.3(c). A noncommercial restriction, an
ethical-use restriction, or a ban on a business model does not fit the list,
and Section 5.3(c) forbids it even if someone tries to describe it as an
extra obligation.

The sentence that ties the list to "GPLv3 Section 7(b)" does not match either
list. It should not be used as a definition. See
[open question 2](../open-questions.md).

## OSI as the approval anchor

The draft does not maintain its own catalog of free licenses. It points at
OSI's approved list, and then applies the Section 1.7 tests on top. OSI
approval is necessary under this draft. It is not sufficient.

That choice avoids freezing a list in 2026, and it refuses non-OSI texts such
as source-available or use-restricted licenses. The cost is a moving target
and a dependency on another organization's process. EUPL-1.2's appendix and
MPL-2.0's secondary-license clause show the other design. The
[roadmap](../../ROADMAP.md) treats a possible fixed list as a supplement or
a replacement, not as a decision already made.

## Relationship to the OSD argument

The replacement right is written as an option exercised by the recipient at
distribution time. It is not a duty to leave OSEL, and it is not a power of
the original licensor to recall rights. The drafting position on OSD
criterion 3 is that "must allow" distribution under the same terms is
satisfied while distribution under OSEL remains available.

Section 5.2 then makes the recipient's own election sticky for that recipient
and that replaced version. The intended analogy is an election the recipient
makes, similar to choosing to publish a derivative under a copyleft license
when the upstream license permits it. Whether a reviewer accepts that analogy
is an open compliance question, not a fact this repository can settle.
