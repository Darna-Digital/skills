1. check the git changes
    - `git status`
    - `git diff`
2. add them
    - `git add .`
3. generate a concise but descriptive message with a title and bullet list of changes
    - `git status --porcelain`
    - `git diff --staged`
4. infer the task number from the branch if available, for example: HNV-123
    - `git branch --show-current`
5. don't include "generated with claude"
6. If available, ensure that the commit is prefixed with the task number from the branch.
7. Commit structure: title + bullet points for changes.
8. don't ask for permission just add changes, describe and commit
9. focus on explaining business value in each bullet point, but don't be too flamboyant.
10. do it fast
