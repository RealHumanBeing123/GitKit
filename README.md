# GitKit

Like cURL Craft, but for Git, and still offline. The HTML file is all that you need.

Pick a command, choose your options, and get a ready-to-run `git` command that updates as you go. Nothing is sent anywhere: the page makes no network requests.

Commands covered:
- Getting started: clone (depth, single branch, submodules, partial and sparse clones) and init.
- Everyday work: status, add, commit (amend, sign-off, GPG, author, date), push, pull and fetch.
- Branches: branch (list, create, rename, delete, set upstream), switch, merge and rebase (including continue, skip and abort).
- Looking around: log (graph, filters by author, message and date, custom formats) and diff (staged, between two refs, name-only, word diff).
- Fixing mistakes: stash, restore, reset, revert and cherry-pick.
- Housekeeping: tag (simple, annotated, signed), remote and clean.
- Run options: run in another folder (`git -C`), temporary settings (`git -c`) and no pager.

Beyond the options themselves, I added a few more things:

- Explanation panel: it breaks the command into parts and says what each one does.

- Quick-start recipes: 16 examples such as a safer force push, a shallow clone, a pretty history graph, undoing the last commit and keeping your changes, and stashing new files too.

- Shell and syntax choices: bash/zsh, PowerShell or cmd, with the right quoting, and short or long flags.

- Warnings: for rewriting history (rebase, `reset --hard`, force push), deleting untracked files, amending a commit that may already be pushed, a missing commit message, an over-long first line and a missing remote name.

Only the options for the command you pick are shown, so the page stays short. `git clean` starts in preview mode (`-n`) so nothing is deleted by accident.

Less common features (worktrees, bisect, submodule commands, sparse-checkout details, hooks) are left out. See `git help` for those.

Just open `GitKit.html` in any browser. It works with no internet connection.
