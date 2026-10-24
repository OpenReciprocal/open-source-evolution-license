# The evolution idea

This page states the idea OSEL exists to carry. It is not the license.
Version 0.1 gestures at the idea and leaves it open.
[`LICENSES/OSEL-0.2-draft.txt`](../LICENSES/OSEL-0.2-draft.txt) writes the
same idea as a closed mechanism. That file is a discussion draft. It does
not amend 0.1. Neither draft is OSI-approved. This page is not legal advice.

简体中文说明在 [zh-CN-idea.md](translations/zh-CN-idea.md)。两份说明不一致时，
以本页英文为准。许可证正文与说明不一致时，以许可证正文为准。

## One sentence

Any recipient may ship a copy under a stricter OSI-approved license drawn
from a fixed menu of duties. Those stricter terms stick to that copy and to
copies made from it. No one may ship that sticky copy under a weaker
license. No other copy is rewritten.

The maintainer does not own the future of the line. The future also cannot
run backward.

## What is conserved

Four things stay in every generation.

1. Anyone who receives the software may use it, study it, modify it, and
   pass it on, including for a fee, in any field.
2. The patent promise a contributor already made stays in force for the
   claims that promise covered. A later evolution does not shrink it, and
   does not widen it onto a contributor who did not make a wider promise.
3. Copyright notices and the text of each license the line has lived under
   stay in the distribution. The past is readable.
4. An ancestor copy stays on the terms it was shipped under. Evolution
   attaches only to the copy named in the record, and to copies made from it.

## What can change

One thing. When a recipient distributes a modified copy that is still under
OSEL, that recipient may bind that copy to an Evolution Target. Section 5.5
of the 0.2 draft calls this copy-level stickiness. The same version label
in someone else's hands is a different copy and stays where it was. Material
taken from the sticky copy carries the stickiness. Deleting the record does
not wipe it off.

An Evolution Target is an unmodified OSI-approved license that does all of
the following:

- keeps the notice duty;
- adds at least one duty from the Evolution Menu;
- adds no duty from outside the Menu;
- does not restrict a field, a person, a group, or a business model.

Taking away the permission to re-license a descendant under a thinner
license is part of making a share-alike or source duty real. The 0.2 draft
says so. Version 0.1 does not, and its sublicense clause can be read as a
way around the whole mechanism.

## The Menu

The Menu is OSEL's own list. It is the creative object. A catalog of license
names would be a different instrument. The Menu admits only these added
duties:

| | Kind of duty | What it covers |
| --- | --- | --- |
| (i) | Attribution | Notices and credit, beyond the notice OSEL already requires |
| (ii) | Source | When, to whom, and in what form source is disclosed, including share-alike |
| (iii) | Patents | A patent grant, retaliation, or a patent defense |
| (iv) | Names | Trademark, or use of a name to endorse a modified version |
| (v) | Changes | Marking a modified version, or describing what changed |

A duty outside the Menu ends the inquiry. The distribution has not evolved.
Typical outsiders: a noncommercial limit, an ethical-use ban, a nationality
ban, a fee for the license itself, a waiting period before the source is
free, a requirement that unrelated programs on the same medium use a given
license.

A governing-law or venue clause is not a Menu duty and is not the extra duty
that qualifies a target. The 0.2 draft says to ignore it for the Menu test,
so a license is not admitted or rejected on the strength of its choice of
court.

## The record

The step exists only when a copy is shipped with an evolution record.
A blog post, a vote, or a commit message does not evolve anything.

In the 0.2 draft the record is `EVOLUTION.md` in the root of a source tree,
or an equally prominent notice when the medium has no root. The record names
the ancestor license, the version that is evolving, the target, the Menu
entries relied on, and the recipient who is taking the step. Older stanzas
stay. The file is a log, not a sticker that replaces yesterday's sticker.

Version 0.1 asks for `LICENSE-REPLACEMENT.md` and only for a tree with a
root directory. That filename describes a generic relicensing. The 0.2 name
describes the act this project is about.

## Three scenes

**Northwind 1.0.** The maintainer ships a library under OSEL. No record is
added. Every recipient may ship their own builds under OSEL. Evolution is a
power the license gives them. Nothing in the license forces them to use it.

**Northwind 2.0, one shipped copy.** A recipient adds a scheduler, ships a
copy labeled 2.0, and includes a valid record naming an OSI-approved
share-alike license whose extra duties sit on the Menu. That copy, and
copies made from it, stay under the target. People who already have 1.0
still have 1.0 under OSEL. Another recipient who builds a different 2.0
from the OSEL sources still holds an OSEL copy, and may ship it under OSEL
or evolve that other copy on its own record. The first recipient cannot
offer the sticky copy under MIT. Contributors allowed the step when they
submitted code. They do not sign a second grant.

**The steps that do not happen.** A recipient announces that Northwind is now
noncommercial. No evolution occurs: the restriction is off the Menu. A
recipient ships a verbatim copy and calls it evolved. No evolution occurs:
0.2 allows the step only for a modified version, so the ancestor and the
verbatim copy stay on OSEL. A recipient fills in a target but cannot point
to a Menu entry that the target actually adds. No evolution occurs. Offering
that version only under the failed target is a breach by that distributor.
Everyone who received the software under OSEL keeps the OSEL grant.

## Why the Menu, and not a list of names

A fixed list of license names goes stale, and it hides the policy inside
other people's documents. The Menu states the policy in OSEL's own words:
added duties may concern credit, source, patents, names, and change-marks.
Anything else is a different kind of license, even if some registry has
approved it.

The cost is that a recipient must map a target onto the Menu before
shipping. The 0.2 draft does not do that mapping in advance, and it does not
declare any particular license to be a target. A map that pretends to be
complete would freeze the Menu into the name-list this draft refuses to be.
The working notes for 0.1 remain in
[known-compatible-licenses.md](compatibility/known-compatible-licenses.md),
and they are about 0.1's test, which is a different and harsher sentence.

## What version 0.1 left unable to close

0.1 calls the step Replacement. It then requires the target's set of
obligations to strictly contain OSEL's set. Real licenses are not nested
that way, so the sentence admits no ordinary license, and the idea cannot
be practiced. 0.1 also grants a sublicense that can be read as permission to
drop to MIT. An idea that can be stepped around is not yet a mechanism.

The 0.2 draft replaces that pair with the Menu test, closes the sublicense,
and states the patent rule the 0.1 notes already asked for: evolution does
not enlarge the original contributor's patent grant. The evolving recipient
may pass on patent terms only for rights that recipient holds.

Clause-by-clause suggestions that fed the draft are still in
[proposed-0.2.md](rationale/proposed-0.2.md). Where the draft and those
suggestions differ, the draft is the assembled text.

## What this page will not turn into

A certification opinion. A promise that OSI will approve either draft. A
recommendation to use OSEL when an existing license already does the job the
maintainer actually wants. The job OSEL is for is the sentence at the top.
A project that wants share-alike from the first tag, or a patent grant and
nothing more, wants a different license. The
[comparison](comparison/comparison-with-other-licenses.md) is reference
material for that choice. It is not the idea.
