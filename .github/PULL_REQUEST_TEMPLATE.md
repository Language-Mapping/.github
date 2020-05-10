<!-- PLEASE REMOVE ANY INAPPLICABLE SECTIONS! -->

## Issues resolved by this pull request

<!--

  The vast majority of pull requests will close one or more issues. These
  should be indicated in list format for better readability and to guarantee
  that they will be automatically closed once this pull request is processed:

  * Fixes #27
  * Fixes #21
  * Fixes #44

-->

- Fixes #

## Prerequisites

<!--

  If relevant, indicate any steps the reviewer must complete in order to process
  the request. Note that these steps are NOT items to review but rather a set of
  pre-review instructions which must be undertaken before the actual review can
  occur. Examples include:

  * Checking out a new branch and pushing some changes to test GitHub Actions
  * Intentionally producing an error locally
  * Installing a particular IDE extension

  It is also important to note that things like "Run a `git fetch` then check
  out this branch" should not be included as these steps are implied.

  Instructions should be provided as an ordered list if more than one step is
  present:

  1. Step 1
  2. Step 2
  3. Step 3

-->

## Review type

<!--

  While pull requests frequently cover multiple scenarios, they generally fall
  into one or more of the following categories:

  * DEPLOYED changes, which can be reviewed for front-end PR's at URLs like
    https://pr-THIS_PR_NUMBER.d3pqoo7mq9yhwf.amplifyapp.com where THIS_PR_NUMBER
    is the current PR ID. This can be found using the link in the "Details"
    section of the "AWS Amplify Console Web Preview" section below, then the
    "View more details on AWS Amplify (us-east-1)" after that. These are
    typically front-end changes which can be reviewed from a browser and may not
    require any `git` steps.
  * LOCAL changes, which require the reviewer to check out the branch in
    question and review something in their local development environment.
  * GITHUB changes, which can typically be reviewed in the browser via the diffs
    and rendered Markdown HTML output.

  The request author simply needs to indicate via "Y" or "N" which type/s apply
  in the table below.

-->

|  **Type**  | **Required (Y/N)** |             **Instructions**             |
| :--------: | :----------------: | :--------------------------------------: |
| `Deployed` |        Y/N         |   Click link near `Deployed to` below.   |
|  `Local`   |        Y/N         | Check out this branch, run its start cmd |
|  `GitHub`  |        Y/N         |     Review diffs and likely Markdown     |

## Items to ignore

<!--

  Help the reviewer out by instructing them to overlook these items as they are
  not yet ready for review. For example, this may include existing issues
  related to the current issue/s being fixed, or it may involve desired design
  enhancements on an issue which only addresses functionality.

  * Use list format...
  * ...if more than one item exists.

-->

## Issue-specific review items

<!--

  If this is not already sufficiently defined by the issue/s to be closed,
  describe the items requiring review. Use **checkboxes** instead of lists here
  as they allow GitHub to display "tasks completed" information.

  * [ ] Use checkboxes...
  * [ ] ...to show overall progress at the top of the page.

-->

- [ ] All checkboxes in the issue/s mentioned have been completed.
- [ ] The issue/s in this request have been resolved.

## General, standard review items

<!--

  INSTRUCTIONS: as a general rule, don't mess with anything from here down
  unless you need to remove something (which will likely be the case for most
  pull requests). The idea is to cover all the bases and reduce the chance of
  the reviewer overlooking something important that should be routinely checked.

-->

### Errors

<!--

  This section does NOT include continuous integration pipelines, which are
  assumed to complete successfully before a pull request is even looked at.

-->

- [ ] **Front-end:** no DevTools console errors occur in the built code (PR
      review URL) in the step/s required to test the PR.
- [ ] **Local/terminal:** no terminal errors occur in the step/s required to
      test the PR.

### Style changes

- [ ] Cohesive **visual design** is preserved relative the rest of the site.
      Colors, type, and layout blend appropriately with the surrounding
      elements.

### Content changes

<!--

  This section covers content-specific items to review but does not address
  in-code proofreading of documentation.

  For spell-checks, consider suggesting an online tool such as SpellBoy:
  https://www.spellboy.com/check_spelling/

-->

- [ ] Content is free of typos, grammar/spelling mistakes, and unclear wording.
- [ ] **README sections:** document outline makes sense semantically (proper use
      of heading levels, lists, tables, etc.).
- [ ] **README formatting:** proper use of `code`, _/paths/to/files/and.stuff_,
      and **emphasis** when needed.
- [ ] **README links:** all links work correctly and any internal links are
      relative.
- [ ] **README headings:** should be "First word capitalized" rather than "Some
      Kind of Other Approach", and should have **unique names** (a Markdown
      linter will catch this).

### Code changes

<!--

  This section covers the code-specific items to review such as:

  * Formatting/syntax
  * Naming conventions for files, variables, functions, etc.
  * In-code documentation

  Note that this primarily applies to NEW code only, and the reviewer should
  exercise some level of leniency by taking that into consideration. If there is
  a good opportunity for the request author to document existing code in close
  proximity to code that has been modified for this request, excellent. But it
  should not be a requirement to fix old undocumented messes (unless of course
  that is the purpose of the issue being resolved).

  The goal for this type of code review is not to create a hassle for the
  developer, but rather to get them to answer "yes" to one question:

  "IF YOU WERE TO READ YOUR OWN CODE A YEAR FROM NOW, WOULD YOU UNDERSTAND IT?"

  Future-proofing code is one of the most challenging aspects of development,
  but with a solid foundation of basic standards and consistent code review the
  process should ultimately become more natural and consistent.

-->

#### Documenting scripting languages

- [ ] Any new `function` is documented using a `docblock`. Existing functions
      that were modified can be addressed on a case-base basis.
- [ ] Each new file has a page header indicating the file's name and a summary
      of what it does.
- [ ] No typos, grammar/spelling mistakes, or unclear wording.
- [ ] Sufficient non-`docblock` documentation is also provided. (e.g. a simple
      `// Smaller headings for About page`).
- [ ] No ambiguous abbreviations are used for variable names. No one, including
      the code author, will know what `const f` refers to at first glance, but
      _everyone_ should know what `const filePath` refers to (or at least have a
      rough idea).

#### Conventions

<!--

  From a broader perspective, this section covers general best practices in
  terms of code maintenance and upkeep. Some core tenets include:

  * Consistent formatting/syntax
  * Intuitive, consistent naming conventions for files, variables, functions,
    etc.
  * DRY code ("don't repeat yourself")

-->

##### Best practices

- [ ] If a _new file_ was created, it is in an appropriate directory.
- [ ] If _new functionality_ was added, the code is in an appropriate file.
- [ ] Efforts have been made to promote _DRY_ code: "don't repeat yourself". If
      the same code has been repeated multiple times, is there a more efficient
      and maintainable way to implement it?
- [ ] Are _naming conventions_ intuitive and consistent with the rest of the
      project?
