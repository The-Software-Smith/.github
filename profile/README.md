# Welcome to the SoftwareSmith Team! 👏🏻

## Repo Guideline
1. Prefer monorepos over polyrepos.
2. Use **kebab-case** when naming new repositories. Make sure to use an appropriate prefix (ike).
3. In the settings, disable 'Issues' and 'Wiki' (replaced by Linear app and Notion respectively).
4. Disable "Rebase and merge" and "Squash and merge" buttons for consistent merge strategies.
5. Enable branch protection and status checks for develop and main branches.

## Contribution Guideline
1. Avoid storing binaries in git, use S3 instead.
2. Follow the project's code style guidelines for consistency.
3. Include Linear issue number in commit messages using the Conventional Commit format.
4. Adhere to GitFlow with main and develop branches, feature, release, and hotfix branches.
5. Require status checks to pass before merging
