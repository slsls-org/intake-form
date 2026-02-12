# Branch Protection Configuration

This document describes the branch protection rules that should be configured for this repository.

## Recommended Settings for Main Branch

To properly protect the `main` branch, the following settings should be configured in GitHub repository settings:

### Access: Settings → Branches → Branch protection rules

1. **Branch name pattern**: `main`

2. **Protect matching branches**:
   - ✅ **Require a pull request before merging**
     - ✅ Require approvals: 1 (at minimum)
     - ✅ Dismiss stale pull request approvals when new commits are pushed
     - ✅ Require review from Code Owners
   
   - ✅ **Require status checks to pass before merging**
     - ✅ Require branches to be up to date before merging
     - Add required status checks: `Validate Changes`
   
   - ✅ **Require conversation resolution before merging**
   
   - ✅ **Do not allow bypassing the above settings**
     - This ensures even administrators follow the same process

3. **Additional recommended settings**:
   - ✅ Restrict who can push to matching branches
     - Configure this to limit direct pushes to only designated team members or CI/CD systems
   - ✅ Allow force pushes: **Everyone** (disabled)
   - ✅ Allow deletions: **Disabled**

## How to Configure

Repository administrators can configure these settings by:

1. Going to the repository on GitHub
2. Click **Settings** (requires admin permissions)
3. Click **Branches** in the left sidebar
4. Click **Add branch protection rule**
5. Enter `main` as the branch name pattern
6. Configure the settings as described above
7. Click **Create** or **Save changes**

## Benefits of Branch Protection

- **Code Quality**: All changes are reviewed before merging
- **Stability**: Prevents accidental or untested changes from breaking the main branch
- **Documentation**: Pull requests provide a history and context for all changes
- **Collaboration**: Facilitates team discussion and knowledge sharing
- **Automation**: Ensures automated tests and checks run before merging

## Current Status

This repository includes:
- ✅ CODEOWNERS file for automatic reviewer assignment
- ✅ GitHub Actions workflow for automated checks
- ✅ Contributing guidelines for developers
- ⚠️  Branch protection rules must be configured in GitHub repository settings (requires admin access)

## For Repository Administrators

To enforce branch protection, you must have admin access to the repository and configure the settings as described above in the GitHub web interface. These settings cannot be version-controlled in the repository itself.
