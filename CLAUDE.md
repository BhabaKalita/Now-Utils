# Now Utils — Claude Code Instructions

## Git Workflow

Every change, no matter how small, must follow this branch-and-merge workflow:

1. **Start from main** — always branch off the latest `main`:
   ```
   git checkout main && git pull
   git checkout -b <descriptive-branch-name>
   ```
2. **Make changes and commit** on the feature branch.
3. **Merge into main** when the change is complete:
   ```
   git checkout main
   git merge --no-ff <descriptive-branch-name>
   git push
   ```
4. **Push the feature branch** to remote as well so there is a record:
   ```
   git push origin <descriptive-branch-name>
   ```

Never commit directly to `main`.

### Branch naming convention
- `feature/<short-description>` — new functionality
- `fix/<short-description>` — bug fixes
- `chore/<short-description>` — non-functional changes (docs, cleanup, config)

## Repository
Remote: https://github.com/BhabaKalita/Now-Utils.git  
Default branch: `main`  
Active account: `BhabaKalita` (switch with `gh auth switch --user BhabaKalita` if needed)
