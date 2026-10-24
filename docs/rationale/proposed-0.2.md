# Proposed clarifications for a later draft

Status: discussion text. These paragraphs are the clause bin that fed
[`LICENSES/OSEL-0.2-draft.txt`](../../LICENSES/OSEL-0.2-draft.txt).
Where this file and that draft differ, the draft is the assembled text.
Version 0.1 is unchanged. Nothing here amends 0.1.

Each proposal names the [open question](../open-questions.md) it responds to.
Wording is suggestive. It has not been adopted.

## Proposal 1. Restate the obligation test

Responds to open questions 1 and 12.

Replace the two sentences of Section 1.7(b) with a test a reader can apply:

> (b) Relative to a distribution under this License with no replacement, the
> candidate license adds one or more duties that fall under Section 1.7(c),
> and it does not remove the notice duty in Section 2 or the patent
> pass-through duty in Section 3.3. Withdrawing permission to sublicense
> under a less restrictive license is allowed and does not fail this test.

A fixed list of license names may be added beside this test. A name on the
list would still have to be OSI-approved at the time of replacement. A name
not on the list would not be a Compatible License, even if the test above
seemed to fit. That is the EUPL and MPL approach, and it is a product choice
as much as a drafting choice.

## Proposal 2. Delete the inaccurate GPL cross-reference

Responds to open question 2.

Delete the sentence "These categories refer to the enumerated list of
acceptable additional terms in Section 7(b) of GPLv3."

If a cross-reference is kept, say only that categories (i), (iv), and (v)
overlap in subject matter with GPLv3 Section 7(b), 7(c), 7(d), and 7(e), and
that categories (ii) and (iii) do not come from that list.

## Proposal 3. Close the sublicense gap

Responds to open question 3.

Add at the end of Section 2(e):

> A sublicense of a modified version or derivative work must be granted under
> this License or under a Compatible License. It must not remove the
> conditions of this License except through a replacement that meets
> Section 5.

## Proposal 4. Define the missing terms

Responds to open question 4.

Add definitions along these lines:

> "Contribution" means work submitted by a Contributor for inclusion in the
> Software, other than communication marked "Not a Contribution."
>
> "Copyright Holder" means a person who holds copyright in the Software or in
> a Contribution. Each Copyright Holder licenses only the work in which that
> Copyright Holder holds copyright.
>
> "Project" means the software project that distributes the Software under
> this License. "Project maintainers" means the people or entity the Project
> identifies as authorized to receive Contributions.
>
> "Affiliate" means an entity that controls, is controlled by, or is under
> common control with a Recipient, where control means ownership of more than
> fifty percent of the voting rights.
>
> "Target License" means the Compatible License named in a valid replacement
> notice under Section 5.1(c).

## Proposal 5. Limit the patent election

Responds to open question 5. This follows the improvement already sketched in
the 0.1 drafting notes, and adds the non-enlargement sentence.

Replace the middle of Section 3.4 with:

> Exercise of the replacement right does not enlarge the patent license the
> original Contributor or Copyright Holder granted under Section 3.1. A
> Recipient may pass downstream the patent provisions of the Target License
> only as to patent rights that Recipient itself has the power to license.
> Those provisions may be used in place of this Section only if they give
> recipients protection no weaker than Section 3.1, and only if they leave
> Section 3.2 in effect for the original Contributor's grant.

## Proposal 6. Say what irrevocable means

Responds to open question 6.

Add to Section 9:

> "Irrevocable" means that the Copyright Holder or Contributor cannot withdraw
> a granted license at will. It does not limit termination under Section 3.2
> or Section 8.

## Proposal 7. Narrow the contributor confirmation

Responds to open question 7.

Replace Section 4.1(c) with a representation of authority and originality,
in the manner of Apache-2.0 Section 5, and delete the general confirmation
that the contribution infringes no third-party intellectual property.

Keep the sentence only if the project decides, in writing and in an issue,
that contributors should bear a non-infringement representation. The default
proposal is to remove it.

## Proposal 8. Make the replacement notice medium-neutral

Responds to open question 8.

Keep `LICENSE-REPLACEMENT.md` in the root directory as the required form for
a source tree. Add:

> If the form of distribution has no root directory, the Recipient must
> include the same four items in another notice that a recipient of that
> distribution would ordinarily see before or with the Software. A source
> tree that has a root directory does not qualify for this alternative.

## Proposal 9. Give the replacement priority over Section 9.3

Responds to open question 9.

Add to Section 9.3:

> A valid replacement under Section 5, the Target License, and the surviving
> provisions in Section 5.4 are part of the terms applicable to the replaced
> version. This Section does not exclude them.

## Proposal 10. Split the disclaimer from the liability limit

Responds to open question 10.

Leave the warranty disclaimer in Section 6. Delete the second sentence of
Section 6, the short liability limit, and leave Section 7 as the only
limitation of liability. Do this only as part of a new version. Existing
0.1 text should stay intact so that copies already in use do not diverge
silently.

## Proposal 11. Notice and cure

Responds to open question 13.

Add:

> Written notice of breach may be given by any Copyright Holder of the work
> concerned, or by a Project maintainer. Notice is effective when sent to an
> address the Recipient has published for legal notices, or, if none, when
> sent to the address from which the Recipient distributed the Software.
> Cure restores rights under this License only. It does not undo a
> replacement already validly exercised.
