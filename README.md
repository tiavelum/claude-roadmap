# claude-roadmap

The roadmap for working with Claude autonomously and economically: one vision issue, the building blocks that lead to it, and the ideas and decisions on the way. It is for tiavelum and for the Claude sessions that work in tiavelum's repositories.

## What it is for

It keeps the plan, the ideas and the decisions that span tiavelum's repositories in one place, so that a session in any of them knows where to put an idea and where to find what is decided.

Everything here is a GitHub issue; the files only say how the issues are used. The work of a building block happens in its own repository, not here.

## Getting started

Open the pinned vision issue, [tiavelum/claude-roadmap#2](https://github.com/tiavelum/claude-roadmap/issues/2). Its sub-issues are the building blocks. Then look at the [open ideas](https://github.com/tiavelum/claude-roadmap/issues?q=is%3Aopen+label%3Aidea) and the [open decisions](https://github.com/tiavelum/claude-roadmap/issues?q=is%3Aopen+label%3Adecision).

To add an issue, choose [New issue](https://github.com/tiavelum/claude-roadmap/issues/new/choose) and pick the form for an idea, a decision or a building block.

## Labels

| Label | Marks | Used in |
|---|---|---|
| `vision` | The pinned vision issue | This repository |
| `idea` | A raw idea, not yet a building block | This repository |
| `decision` | One decision with its options and reasons; closed when made | Any repository that takes part |
| `needs-tiavelum` | A planned touch point that needs tiavelum | Every repository that takes part |

A repository takes part once its issues are building blocks of the vision or steps of one. It needs the `needs-tiavelum` label, and `decision` when it holds decisions, with the descriptions above.

How a touch point is planned, asked and answered is defined by [tiavelum/claude-roadmap#3](https://github.com/tiavelum/claude-roadmap/issues/3).

## Issue hierarchy

- **Vision**: one issue, labelled `vision` and pinned. It states the lighthouse.
- **Building blocks**: the sub-issues of the vision issue. Each lives in the repository where its work happens; one whose repository does not exist yet lives here and is transferred once it does.
- **Steps**: the sub-issues of a building block, in its repository, ordered by "blocked by" links.
- **Ideas and decisions**: issues of their own. An idea has no parent. A decision lives in the repository whose work it decides, and is linked from the issue that waits on it.

## Life of an idea

1. **Captured**: a new issue here, labelled `idea`, from the idea form, wherever the idea came up.
2. **Decided** by tiavelum, one of two ways:
   - **Building block**: the issue loses the `idea` label, gets the building block's sections, becomes a sub-issue of the vision issue, and moves to its repository once that exists.
   - **Not planned**: the issue is closed as not planned, with a comment saying why.

An idea kept for later stays open, with a comment naming what would bring it back, as in [tiavelum/claude-roadmap#5](https://github.com/tiavelum/claude-roadmap/issues/5).

## Life of a decision

A decision issue is opened from the decision form, with every known option, its consequence, a recommendation and the reason. tiavelum answers in a comment, and the issue is closed with the chosen option. Where the decision constrains future work, it is also recorded as a decision record in the repository it concerns.

## Files

| Path | Contains |
|---|---|
| [project-instructions.md](project-instructions.md) | Rules for Claude sessions working here; Claude Code reads it through [CLAUDE.md](CLAUDE.md) |
| [.github/ISSUE_TEMPLATE/](.github/ISSUE_TEMPLATE/) | The forms for an idea, a decision and a building block |
| [.editorconfig](.editorconfig), [.gitignore](.gitignore) | Editor and git settings |

## License

MIT. See [LICENSE](LICENSE).
