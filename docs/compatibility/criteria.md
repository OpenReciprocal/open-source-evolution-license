# Compatible License criteria

Section 1.7 is the gate for the replacement right. A target has to pass every
part of it. Section 5.3 then repeats three prohibitions. This page is a
reading guide for that gate. It does not decide that any particular license
passes. The [working list](known-compatible-licenses.md) applies the guide
and leaves the results unresolved where the text is unresolved.

This page is not legal advice.

## The conditions are cumulative

A Compatible License must satisfy all of the following.

1. It is an OSI-Approved License as Section 1.5 defines that term (Section 1.7, opening, and Section 1.7(a)).
2. It is not a modified OSI license with extra restrictions (Section 1.7(a)).
3. Its obligations are more numerous or more specific than OSEL's, and its obligation set strictly contains OSEL's (Section 1.7(b)).
4. Every additional requirement falls inside Section 1.7(c)(i) through (v).
5. It is not excluded again by Section 5.3, including the ban on field, user, and business-model restrictions.

Failing one condition is enough. There is no balancing test in the draft.

## Step A. OSI approval, unmodified

Section 1.5 requires certification by the Open Source Initiative and presence
on OSI's official list. It also says the license must satisfy all ten OSD
criteria, and it gives four examples. In ordinary cases, approval and the OSD
requirement are the same fact. The extra sentence matters if a reader believes
an approved license misses a criterion. The draft does not say who decides
that dispute.

Section 1.7(a) rejects a modified text. Adding a rider, an exception that
imposes a restriction, or a "Commons Clause" style addendum produces a
different license. That different license is not the OSI-approved text, so
it fails both Section 1.7(a) and Section 5.3(a). An additional permission
that only removes a duty is not an "additional restriction," but it may then
fail Section 1.7(b), because the result is less strict rather than more.

Official texts, not a project's paraphrase, are what Section 5.1(c)(ii)
should point to.

## Step B. Stricter, and strictly containing

Section 1.7(b) has two formulations.

The first is comparative and informal: more obligations, or more specific
obligations, rather than fewer or none.

The second is formal: the target's set of obligations strictly contains
OSEL's set. Equal sets fail. Smaller sets fail. A different shape that is
not a superset fails, even if it feels stricter.

OSEL's own distributor duties, for someone who does not replace, are small:

- keep the copyright notice and the license notice on copies and substantial
  portions (Section 2);
- pass the Section 3 patent grant through, and do not add stricter patent
  restrictions (Section 3.3).

Contributor-only statements in Section 4 are not duties of every downstream
distributor. Section 5 duties apply only when replacement is exercised, so
they cannot usefully be part of the set the target is asked to contain. If
they were, no target could pass, because a target does not require a further
OSEL-style replacement file.

The formal test is still hard, for reasons that do not depend on that
classification:

- Copyleft withdraws the Section 2(e) permission to sublicense on permissive
  terms. Withdrawing a permission is not the same act as adding an
  obligation. The draft wants that withdrawal. The words "strictly contains
  the set of obligations" do not say it counts.
- A target can add a patent license and also regulate patents differently,
  so the patent duties are not nested.
- A target can be stricter about source and looser about some notice. The
  informal sentence might pass and the formal sentence might fail.

This is [open question 1](../open-questions.md). Until a later version
restates the test, a careful recipient does not have a determined "yes" for
any target. The exclusions in Section 5.3(b) are usable now: a license with
fewer or equal obligations is a "no."

## Step C. The additional requirements must fit the closed list

Section 1.7(c) allows additional requirements only in these categories.

| Category | Subject | Typical examples, not determinations |
| --- | --- | --- |
| (i) | Attribution, source attribution, copyright notices | NOTICE files, retained copyright headers |
| (ii) | Scope, timing, or manner of source disclosure, including copyleft | Source with binaries, share-alike, network-use source duties |
| (iii) | Patent grants, patent retaliation, patent defense | Express patent license, termination on patent suit |
| (iv) | Trademark or name use | No use of the author's name to endorse a derivative |
| (v) | Identification of changes | Change logs, "modified by" notices |

A requirement that does not fit has to be treated as disqualifying, even if
the license is OSI-approved and otherwise stricter. Choice of law, choice of
venue, and a general indemnity are the examples to watch. They appear in some
OSI-approved licenses. They are not listed in Section 1.7(c). The draft does
not say whether an unlisted term that is not an "additional requirement" in
the relevant sense can be ignored. That silence is another reason the working
list does not issue a "yes."

### The GPLv3 Section 7 sentence

The closing sentence of Section 1.7 says these categories refer to the
acceptable additional terms in GPLv3 Section 7(b).

GPLv3 Section 7 allows a limited set of additional terms on material you add:

- (a) a different warranty disclaimer or liability limit;
- (b) preservation of legal notices or author attributions;
- (c) marking modified versions, and no misrepresentation of origin;
- (d) limits on publicity use of names;
- (e) declining trademark rights;
- (f) indemnification of licensors and authors in a narrow case.

OSEL (i) is close to GPL 7(b). OSEL (iv) is close to GPL 7(d) and 7(e).
OSEL (v) is close to GPL 7(c). OSEL (ii) and (iii) are not on the GPL list.
GPL 7(a) and 7(f) are not on the OSEL list. The citation also says "7(b)"
when the list runs from 7(a) to 7(f).

Use the five numbered categories as the operative list. Do not use the GPL
sentence to add or remove categories. A later draft should delete or correct
it. See [open question 2](../open-questions.md).

## Step D. Section 5.3 repeats the outer bounds

Even after Section 1.7, Section 5.3 forbids:

- any non-OSI-approved license;
- a license with fewer or equal obligations, naming MIT and BSD, because OSEL
  is modeled on MIT;
- a license that adds restrictions on field of use, users, or business models.

The MIT and BSD examples decide those families. They also decide licenses
that are thinner than MIT, such as a public-domain dedication used as a
license, if someone tried to reach them through replacement. The informal
reason is the same: they do not add obligations.

Section 5.3(c) is about restrictions, not about additional affirmative
duties. A duty to provide source when the software is used over a network
restricts a business only in the sense that compliance has a cost. The OSD
does not treat that cost as discrimination against a field. This page reads
Section 5.3(c) the same way: a prohibition on a field, a class of users, or
a business model fails; a source duty that applies to whoever distributes or
offers the software does not fail merely because a business is among those
persons.

## What the recipient has to be able to write down

Section 5.1(c)(iii) requires a short explanation of the compatibility basis,
citing the Section 1.7(c) categories that the extra requirements fall into.
A notice that says only "GPL is stricter" does not do that. A notice that
cites categories without saying which GPL (or other) provisions fall into
them also does not do that.

Because step B is unresolved, this repository's example notice is a form with
placeholders. Filling it in is a conclusion the 0.1 text does not authorize
this project to make. See
[`examples/LICENSE-REPLACEMENT.md`](../../examples/LICENSE-REPLACEMENT.md).

## Worked pattern, without a conclusion

For a candidate, write the answers in this order:

1. SPDX identifier or official name, and the exact version.
2. URL of the OSI listing and of the official text used.
3. Confirmation that the text is unmodified.
4. The OSEL duties relied on as the contained set. State whether Section 4
   duties are included. Today that choice changes the result, so record it.
5. Each added duty, mapped to one Section 1.7(c) category, or marked as
   unlisted.
6. Any permission the candidate withdraws, especially Section 2(e).
7. Any field, user, or business-model restriction.
8. How the candidate's patent terms relate to Section 3, including whether
   the recipient would need the Section 3.4 election.
9. The result: excluded, or not determined.

Do not write "compatible" at step 9 under version 0.1 unless a later
operative text has settled step B. The honest result for a stricter
OSI-approved license, today, is "not determined."
