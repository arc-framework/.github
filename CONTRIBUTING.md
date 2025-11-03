# Contributing to A.R.C. (Agentic Reasoning Core)

First off, thank you for considering contributing! We're building a "Platform-in-a-Box" for AI agents, and we're excited to have you on board. Every contribution, from a typo fix to a new feature, is valuable.

This document is the "front door" for contributors. Please read it to get started.

## 🤝 Code of Conduct

Before you start, please read our **[CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)**. We enforce this code strictly to ensure A.R.C. is a welcoming and inclusive project for everyone.

## 🤔 How Can I Contribute?

There are many ways to help, and not all of them involve writing code:

* **Reporting Bugs:** Find a bug? Please [open a bug report](https://github.com/arc-framework/.github/issues/new/choose).
* **Suggesting Enhancements:** Have a great idea for a new feature? [Open a feature request](https://github.com/arc-framework/.github/issues/new/choose).
* **Writing Documentation:** Our docs are the most important part of our framework. Help us make them better!
* **Submitting Pull Requests:** Ready to write some code? This guide will walk you through it.

## 🚀 Your First Code Contribution

Ready to dive in? Here's the step-by-step workflow for getting your code merged.

### 1. Find an Issue
A great place to start is our organization's **[Issues tab](https://github.com/arc-framework/arc/issues)**.
* Look for issues labeled **`good first issue`**. These are specifically chosen as a good entry point into the codebase.
* If you want to work on something, **leave a comment** to let us know. This prevents multiple people from working on the same thing.

### 2. Fork & Clone the Repo
Our platform is a collection of many repositories. You'll need to fork and clone the *specific repository* you want to work on (e.g., a specific service, the CLI, or the docs).

1.  Fork the repo (e.g., `github.com/arc-framework/engine`) to your own account.
2.  Clone your fork locally:
    ```bash
    git clone [https://github.com/YOUR-USERNAME/repository-name.git](https://github.com/YOUR-USERNAME/repository-name.git)
    cd repository-name
    ```

### 3. Create Your Branch
We use a **Trunk-Based Development** model. `main` is our only permanent branch. We **do not** use a `develop` branch.

Please create your new branch from the `main` branch, following our organization's naming convention. The convention is to prefix your branch with a "category" tag, followed by a `/`.

* **`feature/`**: For developing a new feature.
* **`bugfix/`**: For fixing a bug.
* **`hotfix/`**: For a critical, urgent bug in production.
* **`docs/`**: For changes to documentation only.
* **`refactor/`**: For code changes that don't add features or fix bugs.

```bash
# Make sure you're on main and have the latest code
git checkout main
git pull origin main

# Create your new branch
git checkout -b feature/my-cool-agent
```

### 4. Write Your Code (and Tests!)
This is the fun part!

Write your code.

Write new tests to cover your changes.

Run the existing tests (look for a README.md in the repo for test commands) to make sure you didn't break anything.

### 5. Sign Your Commits (DCO)
This is a mandatory step. We use the Developer Certificate of Origin (DCO). It's a lightweight, legal way for you to certify that you wrote the code.

It's easy: just add a -s flag to your git commit command.

```bash

# The -s flag adds a "Signed-off-by: Your Name <your.email@example.com>" line

git commit -s -m "feat: add my new cool agent"
PRs with commits that are not signed off will be rejected by our CI.
```

### 6. Open Your Pull Request
Ready to merge? Push your branch to your fork and open a Pull Request (PR) against the arc-framework/main branch.

Fill out the PR template. Explain what you changed and why.

Link the Issue. Make sure to add Closes #123 (or whatever the issue number is) in your PR description.

Be patient. A maintainer will review your code.

### 7. The Review Process
We take our code quality seriously. To get merged, your PR must:

Pass all CI checks (tests, linter, DCO check).

Get at least one approval from a maintainer.

Resolve all conversations. If a reviewer leaves a comment, you must address it (even if it's just to say "Done!") and resolve the conversation.
