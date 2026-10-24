# Contributing

OSEL is a draft specification. A change to the license text changes rights
for anyone who adopts that version. This file separates that kind of change
from editorial work.

By contributing, you agree to the [code of conduct](CODE_OF_CONDUCT.md).

## Licenses of contributions

Two licenses apply, matching [LICENSE](LICENSE).

- If you propose wording for the OSEL license text, you agree that your
  textual contribution to that wording is dedicated under CC0-1.0. The
  license text has to stay freely reusable. A contribution that cannot be
  included under CC0 cannot be merged into `LICENSES/`.
- Documentation, translations, examples, and other non-license material are
  contributed under CC-BY-4.0 unless you state another compatible grant in
  the pull request.

Do not contribute material you do not have the right to submit. Do not
paste another license's text into the OSEL draft except for a short quotation
needed to compare clauses, with the source identified.

## Start with an issue

Open an issue before a substantial change to Sections 1 through 9, the
definitions, or the replacement procedure. Use the license-text template.
The issue should name:

- the section you want to change;
- the behavior you want;
- how the change relates to the Open Source Definition;
- whether it answers an item in [docs/open-questions.md](docs/open-questions.md).

Editorial fixes to documentation, typos in examples, and translation
corrections can go straight to a pull request. If the "typo" changes a
defined term or a grant, it is not editorial.

## Version rules

`LICENSES/OSEL-0.1.txt` is the canonical text of the published 0.1 draft.
`LICENSES/OSEL-0.2-draft.txt` is the discussion draft. Comments on the Menu
belong on that file.

- Do not silently rewrite 0.1 to add a new rule. The 0.2 discussion draft is
  where the Menu is being argued.
- Renaming `OSEL-0.2-draft.txt` to a stable `OSEL-0.2.txt` is a maintainer
  decision that the discussion text has frozen. Do that in its own change,
  with a changelog entry.
- Non-operative notes do not belong in a license file. They belong under
  `docs/`.
- Non-operative notes do not belong in the license file. They belong under
  `docs/rationale/`.

The English text controls. A translation pull request should not introduce
rules that the English text does not contain. Mark the translation
unofficial, which the current Chinese file already does.

## What a license-text pull request needs

1. The issue it closes.
2. A unified change to the plain-text license and the Markdown license.
3. Updates to the annotated spec, the open-question list, and the changelog
   when the answer changes one of those documents.
4. A short OSD note: which criteria you touched, and whether you believe the
   draft position got stronger or weaker.
5. No claim that the result is OSI-approved.

Documentation-only pull requests that "determine" a license to be compatible
will not be merged. Section 1.7 is operative text. The working list can
record an exclusion the current text already supports. It cannot invent a
positive compatibility finding. See
[known-compatible-licenses.md](docs/compatibility/known-compatible-licenses.md).

## Discussion

Comment on the clause, the consequence, and the OSD criterion. The code of
conduct bars personal attacks. It also asks you not to present your view as
legal advice for another contributor.

Maintainers may ask you to shrink a pull request that mixes an editorial
cleanup with a normative change.

## Local preview

This repository is Markdown and plain text. Rendering the files, and checking
that links resolve, is enough. There is no build step.
