# Welcome to the SoftwareSmith Team! 👏🏻

## Repository Creation Guidelines

All new repositories **must** be created using our template repository, **`tss-template`**. This ensures consistency in settings and branch protection rules across the organization.

### Creating a New Repository from the Template

1. **Start from the Template:**
   - Navigate to the **`tss-template`** repository.
   - Click the **"Use this template"** button.
   - When prompted, **select the "Copy all branches" option**. This will ensure that every branch from the template is included in your new repository.

2. **Naming the Repository:**
   - Use **kebab-case** naming for the repository.
   - For project-specific repositories, follow these patterns:
     - **ike-backend**, **ike-frontend**
     - **land-backend**, **land-frontend**  
     _Note: "ike" and "land" are project code names._
   - For repositories not tied to a specific project:
     - Use the prefix **`tss`** (for The Software Smith).
     - Alternatively, use **`poc`** if it is a proof of concept.

3. **Set Default Branch:**
   - The repository’s default branch should be set to **`develop`**.

### Branch Protection Rules

All new repositories must apply the following branch protection rules:

#### 1. **`main` Branch**
- **Require a pull request before merging.**
  - Require at least **1 approval**.
  - **Dismiss stale pull request approvals** when new commits are pushed.
- **Require status checks to pass before merging.**
  - Ensure branches are **up to date** before merging.
- **Require conversation resolution before merging.**
- **Do not allow bypassing the above settings.**

<img width="782" alt="image" src="https://github.com/user-attachments/assets/b1564f1c-e374-4911-8c87-631c81426913" />

#### 2. **`develop` Branch**
- Apply the same rules as the **main** branch.

#### 3. **`feature/*` and `bugfix/*` Branches**
- **Do not allow bypassing the above settings.**
- **Allow branch deletions.**

<img width="792" alt="image" src="https://github.com/user-attachments/assets/4ca5e7dd-80e3-4d67-b3c6-19a4bc0c3329" />

#### 4. **`release/*` and `hotfix/*` Branches**
- **Do not allow bypassing the above settings.**

<img width="787" alt="image" src="https://github.com/user-attachments/assets/506364d8-6cdc-4a07-b6f4-223c74b314fc" />


### Other Repository Settings

- **Merge Options:**
  - Allow **merge commits**.
  - Allow **squash merging**.
  - Allow **rebase merging**.
- **Pull Request Settings:**
  - Always suggest **updating pull request branches**.
- **Branch Cleanup:**
  - Automatically **delete head branches** after merging.

## Contribution Guideline
1. Avoid storing binaries in git, use S3 instead.
2. Follow the project's code style guidelines for consistency.
3. Include Linear issue number in commit messages using the Conventional Commit format.
4. Adhere to GitFlow with main and develop branches, feature, release, and hotfix branches.
5. Require status checks to pass before merging
