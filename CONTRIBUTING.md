# Contributing to Intake Form

Thank you for your interest in contributing to this project!

## Branch Protection and Workflow

### Protected Branches

The `main` branch is protected to ensure code quality and stability. Direct commits to `main` are **not allowed**.

### How to Contribute

1. **Create a new branch** from `main` for your changes:
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** on your feature branch

3. **Commit your changes** with clear, descriptive commit messages:
   ```bash
   git add .
   git commit -m "Description of your changes"
   ```

4. **Push your branch** to the repository:
   ```bash
   git push origin feature/your-feature-name
   ```

5. **Create a Pull Request** (PR) on GitHub:
   - Go to the repository on GitHub
   - Click "New Pull Request"
   - Select your branch as the source
   - Select `main` as the target
   - Fill in the PR description with details about your changes
   - Submit the PR for review

### Pull Request Requirements

- All changes must go through a pull request
- PRs require approval from code owners before merging
- Automated checks must pass
- Keep PRs focused and reasonably sized for easier review

### Code Review Process

1. A code owner will review your PR
2. Address any feedback or requested changes
3. Once approved and all checks pass, your PR will be merged

## Questions?

If you have questions about the contribution process, please open an issue or contact the maintainers.
