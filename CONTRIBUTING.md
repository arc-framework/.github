# Contributing to A.R.C. (Agentic Reasoning Core)

First off, thank you for considering contributing! We're building a "Platform-in-a-Box" for AI agents, and we're excited to have you on board. Every contribution, from a typo fix to a new feature, is valuable.

This document is the "front door" for contributors. Please read it to get started.

## 🤝 Code of Conduct

Before you start, please read our **[CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)**. We enforce this code strictly to ensure A.R.C. is a welcoming and inclusive project for everyone.

## 🤔 How Can I Contribute?

There are many ways to help, and not all of them involve writing code:

* **Reporting Bugs:** Find a bug? Please [open a bug report](https://github.com/arc-framework/arc/issues/new/choose) (this link will be added later) and let us know.
* **Suggesting Enhancements:** Have a great idea for a new feature? [Open a feature request](https://github.com/arc-framework/arc/issues/new/choose).
* **Writing Documentation:** Our docs are the most important part of our framework. Help us make them better!
* **Submitting Pull Requests:** Ready to write some code? This guide will walk you through it.

## 🚀 Your First Code Contribution

Ready to dive in? Here's the step-by-step workflow for getting your code merged.

### 1. Find an Issue
A great place to start is our **[Issues tab](https://github.com/arc-framework/arc/issues)**.
* Look for issues labeled **`good first issue`**. These are specifically chosen as a good entry point into the codebase.
* If you want to work on something, **leave a comment** to let us know. This prevents multiple people from working on the same thing.

### 2. Fork & Clone the Repo
Our platform is a collection of many repositories. You'll need to fork and clone the *specific repository* you want to work on (e.g., `cli`, `gateway`, `engine`).

1.  Fork the repo (e.g., `github.com/arc-framework/engine`) to your own account.
2.  Clone your fork locally:
    ```bash
    git clone [https://github.com/YOUR-USERNAME/engine.git](https://github.com/YOUR-USERNAME/engine.git)
    cd engine
    ```

### 3. Set Up Your Environment
Our platform is polyglot (Go, Python, etc.). The setup for each repo is different.

**Please look for the `README.md` or `CONTRIBUTING.md` file *inside that specific repo* for detailed setup instructions.**
* For **Go** projects (`cli`, `gateway`), you'll need Go 1.21+ and `make`.
* For **Python** projects (`engine`, `processor`), you'll need Python 3.11+, `pip`, and `virtualenv`.

### 4. Create Your Branch
We use a **Trunk-Based Development** model. `main` is our only permanent branch. We **do not** use a `develop` branch.

Please create your new branch from the `main` branch, using our naming convention:
* **Features:** `feature/my-new-feature`
* **Bugfixes:** `bugfix/fix-that-bug`
* **Docs:** `docs/update-readme`

```bash
# Make sure you're on main and have the latest code
git checkout main
git pull origin main

# Create your new branch
git checkout -b feature/my-cool-agent
