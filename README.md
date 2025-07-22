# Programming Starter Pack <small>[Work in progress]</small>

This is a repository for collecting resources to learn programming.

Rhetorical Question: Why should we create our own materials instead of using existing ones?

So, let's gather all the 'best' programming resources here. Over time, we will see which resources are the best and which are not. Of course, what is considered the 'best' is subjective.

Optional topics are not necessary for junior-level knowledge, but they are good to know.

For programming first, you need to select a path.
You need to decide the programming language based on your goals,
what you want to achieve with programming, what you want to program.

For example, for hardware (physical things) programming, you need to learn one of them: C, C++, Rust, etc.
For frontend web development, you need to learn HTML, CSS, and JavaScript.
For backend web development you need to learn one of them: JavaScript, Python, PHP, Java, C#, Go, Rust, etc.
With JavaScript, you can do frontend and backend development too, so it's a good start for web development.
For mobile development, you need to learn one of them: Java, Kotlin, Swift, Dart, etc.

You can find programming roadmaps here: [roadmap.sh](https://roadmap.sh/)

You can read / watch hungarian materials here: [README.hu.md](README.hu.md)

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

- A **pre-push hook** automatically checks for Markdown linting errors before allowing code to be pushed to the repository
- This ensures that all Markdown files maintain consistent formatting
- The hook runs the `lint:md` script to check all Markdown files

If the pre-push hook blocks your push due to linting errors:

1. Run `npm run lint:md` to see the specific errors
2. Fix the errors manually or run `npm run lint:md:fix` to automatically fix issues where possible
3. Commit your changes and try pushing again

# Web-programming starter pack (HTML, CSS, JavaScript)

For learning web-programming, you need to learn HTML, CSS, and JavaScript.
You can learn them in any order, but I recommend learning HTML first, then CSS, then JavaScript.

- [HTML + CSS links](./html-css.md)
- [JavaScript links](./javascript.md)

## Linux / Bash / Command Line (CLI)

- For deploying web applications, you need to know how to use the command line.
- On servers, you will use Linux (most of the time), so you need to know how to use it.
- If you're lucky, then you can avoid learning command line.
  There are providers where you can deploy your application without using the command line.
