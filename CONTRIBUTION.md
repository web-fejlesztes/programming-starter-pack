# Contribution

If you have any suggestions, please create a well-specified issue or pull request.

## Markdown Linter

This project uses a Markdown linter to ensure consistent formatting of Markdown files.
The linter is configured to focus on important formatting issues while allowing flexibility for educational content.

### Setup

The project uses [markdownlint-cli2](https://github.com/DavidAnson/markdownlint-cli2) for linting Markdown files.
If you want to contribute, make sure you have Node.js installed, then run:

```bash
npm install
```

### Usage

To check all Markdown files for issues:

```bash
npm run lint:md
```

To automatically fix issues where possible:

```bash
npm run lint:md:fix
```

Note: The fix command uses the `--fix` flag with markdownlint-cli2, not a separate binary.

### Configuration

The linter configuration is in the `.markdownlint.json` file. It's configured to be permissive for educational content while enforcing some basic formatting rules:

- Files should end with a single newline character
- Other style rules are relaxed to accommodate the project's existing style

When contributing, please make sure your Markdown files pass the linter check or provide a good reason for exceptions.

### Git Hooks

This project uses Git hooks to enforce code quality standards:

- A **pre-commit hook** automatically fixes Markdown linting issues when you commit changes
- A **pre-push hook** checks for any remaining Markdown linting errors before allowing code to be pushed
- These hooks ensure that all Markdown files maintain consistent formatting

If the pre-push hook blocks your push due to linting errors:

1. Run `npm run lint:md` to see the specific errors
2. Fix the errors manually or run `npm run lint:md:fix` to automatically fix issues where possible
3. Commit your changes and try pushing again

### CI Pipeline

This project uses GitHub Actions to automatically check Markdown files in the CI pipeline:

- A workflow runs whenever Markdown files or linter configuration files are changed
- It triggers on both push events to main/master branches and pull requests
- The workflow installs dependencies and runs the `lint:md` script
- This ensures that all Markdown files maintain consistent formatting even if local hooks are bypassed

The CI workflow configuration is in the `.github/workflows/markdown-lint.yml` file. If the CI check fails:

1. Check the GitHub Actions logs to see the specific errors
2. Make the necessary corrections to fix the linting issues
3. Push your changes to trigger the workflow again
