# Contribution Guidelines

Thanks for helping keep this list accurate. Please read this page before opening a pull request.

## What belongs here

An agent belongs on this list when it:

- Runs from a terminal against a local checkout, or is a command-line client for a hosted coding agent.
- Is publicly available today, with a working install path and public documentation or source code.
- Is maintained: the repository is not archived, the project has not announced that it is unmaintained or shutting down, and it has shipped a commit or release in roughly the last six months.
- Is the official project, not a mirror, a rebrand of someone else's work, or a fork without meaningful changes of its own.
- Can be used as distributed. Projects that redistribute code without the right to do so are not accepted.

Editor extensions without a terminal agent, chat-only model wrappers, and general LLM frameworks belong in other lists.

## Entry format

Add one line to the section that fits best:

```markdown
- [Name](https://link.to/official/repo-or-docs) - Maker and what the agent does, in one or two plain sentences. Open source (MIT). Install: `install command`.
```

- Link to the official repository or documentation, not a blog post, package registry page, or marketplace listing.
- Name the maker and say what the agent does. Write the description yourself, and leave out superlatives, rankings, and benchmark claims.
- Label the license as `Open source (SPDX-ID)`, `Source-available (license name)`, or `Proprietary`.
- Mark tools that only run on a Mac with `macOS`.
- Use the install command from the project's own documentation.
- Keep entries alphabetical within the section (case-insensitive). Descriptions start with a capital letter and end with a period.

## Pull requests

- One entry per pull request. Separate pull requests are easier to review and to revert.
- Use the agent's name as the pull request title, and say in the body why it belongs here.
- Check that every link resolves and that the repository is not archived.
- Run `npx awesome-lint` before you push.

## Corrections and removals

Open an issue or a pull request when a link breaks, a project is renamed, archived, or abandoned, or a description has gone stale. Removing dead entries is as useful as adding new ones.
