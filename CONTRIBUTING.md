# Contributing Guidelines

We encourage people to make contributions to this project following these
guidelines. If you are looking for ways to contribute, start with [issues
flagged as "help
wanted"](https://github.com/Language-Mapping/language-map/labels/comm%3A%20%3Araising_hand%3A%20help%20wanted%3Araising_hand%3A).

## Pull Requests

Use the general [open source forking
workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)
to contribute to this project. After a feature is complete, make a pull request
and wait for a repository admin to review and approve your PR.

Try to keep PRs as small and focused as possible. If you are making a big
breaking change in production and don't want to expose half finished
functionality to users, you can use [feature
flags](https://www.martinfowler.com/articles/feature-toggles.html) to work on
this incrementally. If you are making a long, complicated PR, it is likely that
you will be asked to break it into more focused pieces.

### Rebasing

Avoid rebasing and force-pushing once you've opened a pull request. This
rewrites history and makes it more difficult for the person reviewing your code
to see active changes.

## Branches

If a branch corresponds directly to an issue, the branch name should be prefixed
by the issue number and a period followed by a concise slug for the issue name
(e.g. `423.user-avatar`).

If there is no corresponding issue, branch names should start with first letter
of first name + last name, followed by a forward slash, and a descriptive
message that explains the intention of the branch. Words should be separated by
hyphens.

The important part is to use a consistent identifier as the first part of the
branch name that makes it easy to tell who made the branch at a glance.

A good branch name:

```
jsmith/feature-add-world-map
```

Instead of:

```
login
```

## Commit Messages

Commits should use the present, imperative tense. This makes it easier to look
through commit history and encourages cleaner, well thought out commit messages.

Basically your commit message should be able to fit inside this phrase:

```
If applied, this commit will <commit message>
```

For example, `add symbology to counties layer` is in the present-tense,
imperative and reads as: `If applied, this commit will add symbology to counties layer`.

It's easy to remember how to phrase it if you think of a commit message as
giving an order to the codebase.

For a more detailed description of this, see:

- [Stackoverflow post](https://stackoverflow.com/a/3580764/3908605)
- [Official Git
  Documentation](https://git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project)

## Pull Request Guidelines

Not all of this will apply to this project, but the majority of the info
contained in our **Pull Request templates** can be seen in detail
[here](https://raw.githubusercontent.com/Language-Mapping/.github/8550c16ea4ab0e1245763a0b3783eeacabe49d51/.github/PULL_REQUEST_TEMPLATE.md).
