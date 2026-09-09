# commit-push-pr

Commit all staged changes, push to the current branch, and open a pull request.

Steps:
1. Run `git status` to show what will be committed.
1. Run `git diff --staged` to rewiew staged changes.
1. Write a commit message in convetional commit format (e.g. `feat:`:, `fix:`, `chore:`, `refactor:`) based on that is staged.
1. Run `git commit -m <message>` with that commit message.
1. Run `git push origin <current-branch>` using the current branch name.
1. Run `gh pr create --fill --body "<commit-message>"` to open a pull request, using the commit message as the PR body.
