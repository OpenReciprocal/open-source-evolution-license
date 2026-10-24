# Examples

These files show how to apply a draft. They are not part of either license.

- Version 0.1: copy [`LICENSES/OSEL-0.1.txt`](../LICENSES/OSEL-0.1.txt).
  The step, if you take one, uses [`LICENSE-REPLACEMENT.md`](LICENSE-REPLACEMENT.md).
- Version 0.2 discussion draft: copy
  [`LICENSES/OSEL-0.2-draft.txt`](../LICENSES/OSEL-0.2-draft.txt).
  The step uses [`EVOLUTION.md`](EVOLUTION.md).

Do not attach a 0.2 record to software you offered under 0.1.

## Apply the draft

1. Copy `LICENSES/OSEL-0.1.txt` to `LICENSE` in the root of your project.
2. Leave the copyright notice as `Copyright (c) 2026 OpenReciprocal`.
   Do not substitute a personal name.
3. Put the header in [`source-header.txt`](source-header.txt) at the top of
   each source file, adjusted to that file's comment syntax.
4. Do not add "OSI Approved" to the header. Version 0.1 is not approved.

A scanner-friendly identifier is `LicenseRef-OSEL-0.1`. It is not an SPDX
License List identifier.

## Replace the license on a new version

Do this only when you distribute a new version and you have concluded that
the target is a Compatible License under Section 1.7. Version 0.1 of this
project does not reach that conclusion for any target. See
[`docs/compatibility/known-compatible-licenses.md`](../docs/compatibility/known-compatible-licenses.md).

If you do exercise the right:

1. Distribute the new version. A notice without a distribution has no effect
   (Section 5.1(a)).
2. Add [`LICENSE-REPLACEMENT.md`](LICENSE-REPLACEMENT.md) in the root, with
   the four required items and the placeholders filled from your own analysis.
3. Keep the OSEL text and the original copyright notices in the tree
   (Section 5.1(e)).
4. Do not also ship that same version under MIT, BSD, or OSEL again
   (Section 5.2).

The replacement file in this directory uses angle-bracket placeholders on
purpose. It is a form, not a filled notice, because a filled target would
look like a compatibility finding.
