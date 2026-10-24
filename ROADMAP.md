# Roadmap

OSEL 0.1 is a working draft. Dates below are not commitments. An item moves
when the text is ready, not when a calendar date arrives.

## Done in the 0.1 publication

- Permissive grant, patent grant, contributor grant, and replacement right.
- First statement of the Compatible License test and the Section 5 procedure.
- Public draft of 2026-09-26.

## Done as documentation around that draft

- Canonical plain text separated from non-operative notes.
- Annotated specification, OSD checklist, compatibility criteria, working
  list, and comparison.
- Application examples, issue templates, and a Simplified Chinese translation
  of the operative text.
- A written list of open questions and suggested 0.2 wording. The suggestions
  are not the license.

## Now: the 0.2 discussion draft

[`LICENSES/OSEL-0.2-draft.txt`](LICENSES/OSEL-0.2-draft.txt) assembles the
Menu, the closed sublicense, the patent boundary, and the evolution record.
It is open for argument. It is not a retirement of 0.1. The idea it
implements is [docs/evolution.md](docs/evolution.md). Clause notes that fed
it remain in [docs/rationale/proposed-0.2.md](docs/rationale/proposed-0.2.md).

The point of the next round of comments is to attack that draft: Menu
entries that are too wide or too narrow, the treatment of share-alike, and
whether a failed step is stated clearly enough. A fixed list of license
names is a different product. This line of drafts does not adopt one.

## Earlier plan for that draft

The point of 0.2 is to make the 0.1 test decidable and to close the internal
gaps listed in [docs/open-questions.md](docs/open-questions.md). The working
text for that discussion is
[docs/rationale/proposed-0.2.md](docs/rationale/proposed-0.2.md).

In priority order:

1. Restate or replace the strict-superset test.
2. Decide whether a fixed list of target licenses should stand beside the
   test. EUPL-1.2 and MPL-2.0 are the models for a list. Version 0.1 is the
   model for an open test. The project may keep one, or use a list as a
   sufficient condition and the test as a necessary one.
3. Close the Section 2(e) sublicense gap.
4. Define Project, Copyright Holder, Contribution, Affiliate, and Target
   License, and state that each copyright holder licenses only their own work.
5. State that a patent election cannot enlarge the original contributor's
   grant, and that Section 3.2 survives.
6. Correct the GPLv3 Section 7 citation.
7. Make the replacement notice valid for a distribution that has no root
   directory.
8. Say what "irrevocable" means next to Sections 3.2 and 8.
9. Decide whether Section 4.1(c)'s non-infringement sentence stays.

A 0.2 file will be added only when the maintainers are ready to freeze that
wording as a draft. Discussion happens in issues first.

## Possible later steps

These depend on 0.2 or on whatever version first has a stable compatibility
rule.

- More worked distribution examples, including a source tarball and a note
  for a single-file program.
- Further translations, each marked as unofficial, with English controlling.
- An external review by people who are not the maintainers. Comments belong
  in the issue tracker so the record stays with the draft.
- An OSI submission, if the maintainers then believe the text meets the OSD,
  is clear enough to apply, and is distinct enough from MIT, Apache-2.0,
  EUPL-1.2, and MPL-2.0 to justify another license.

A submission is a possible outcome. It is not scheduled. The repository will
not describe OSEL as submitted, or as approved, until that is true.

## Not planned

- Use restrictions, noncommercial riders, or ethical-use clauses. Those
  conflict with OSD criteria 5 and 6 and with Section 5.3(c).
- A proprietary period followed by an automatic flip to OSEL.
- Retroactive amendment of versions that have already been published.
- A claim that the documentation is legal advice.
