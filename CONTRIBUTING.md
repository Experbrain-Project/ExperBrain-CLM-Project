# Contributing to the Cortical Language Model

First off, thank you for considering contributing to the Cortical Language Model! It's people like you that make the CLM such a great project.

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

This section guides you through submitting a bug report. Following these guidelines helps maintainers understand your report, reproduce the behavior, and find related reports.

#### Before Submitting A Bug Report

* **Check the documentation** to see if you can determine the expected behavior.
* **Check the existing issues** to see if the problem has already been reported.
* **Perform a search** to see if a similar issue has already been solved.

#### How Do I Submit A Good Bug Report?

Bugs are tracked as [GitHub issues](https://guides.github.com/features/issues/). Create an issue and provide the following information:

* **Use a clear and descriptive title** for the issue to identify the problem.
* **Describe the exact steps which reproduce the problem** in as many details as possible.
* **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples.
* **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
* **Explain which behavior you expected to see instead and why.**
* **Include screenshots and animated GIFs** which show you following the described steps and clearly demonstrate the problem.
* **Include the version of Python, PyTorch, and other dependencies** you're using.

### Suggesting Enhancements

This section guides you through submitting an enhancement suggestion, including completely new features and minor improvements to existing functionality.

#### Before Submitting An Enhancement Suggestion

* **Check if there's already a package** which provides that enhancement.
* **Determine which repository the enhancement should be suggested in.**
* **Perform a search** to see if the enhancement has already been suggested.

#### How Do I Submit A Good Enhancement Suggestion?

Enhancement suggestions are tracked as [GitHub issues](https://guides.github.com/features/issues/). Create an issue and provide the following information:

* **Use a clear and descriptive title** for the issue to identify the suggestion.
* **Provide a step-by-step description of the suggested enhancement** in as many details as possible.
* **Provide specific examples to demonstrate the steps**. Include copy/pasteable snippets which you use in those examples.
* **Describe the current behavior** and **explain which behavior you expected to see instead** and why.
* **Explain why this enhancement would be useful** to most CLM users.
* **List some other packages where this enhancement exists, if any.**

### Your First Code Contribution

Unsure where to begin contributing to the CLM? You can start by looking through these `good first issue` and `help wanted` issues:

* [Good first issues](https://github.com/ExperBrain-Project/cortical-language-model/issues?q=is%3Aopen+is%3Aissue+label%3A%22good+first+issue%22) - issues which should only require a few lines of code, and a test or two.
* [Help wanted issues](https://github.com/ExperBrain-Project/cortical-language-model/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) - issues which should be a bit more involved than `good first issue` issues.

### Pull Requests

The process described here has several goals:

- Maintain CLM's quality
- Fix problems that are important to users
- Engage the community in working toward the best possible CLM
- Enable a sustainable system for CLM's maintainers to review contributions

Please follow these steps to have your contribution considered by the maintainers:

1. Follow the [styleguides](#styleguides)
2. After you submit your pull request, verify that all [status checks](https://help.github.com/articles/about-status-checks/) are passing

While the prerequisites above must be satisfied prior to having your pull request reviewed, the reviewer(s) may ask you to complete additional design work, tests, or other changes before your pull request can be ultimately accepted.

## Styleguides

### Git Commit Messages

* Use the present tense ("Add feature" not "Added feature")
* Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
* Limit the first line to 72 characters or less
* Reference issues and pull requests liberally after the first line

### Python Styleguide

All Python code must adhere to [PEP 8](https://www.python.org/dev/peps/pep-0008/) and [PEP 257](https://www.python.org/dev/peps/pep-0257/). We use [Black](https://github.com/psf/black) for code formatting and [Flake8](https://flake8.pycqa.org/) for linting.

### Documentation Styleguide

* Use [Google-style docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html)
* Use [Markdown](https://daringfireball.net/projects/markdown/) for all documentation
* Reference methods and classes in backticks: `CorticalLanguageModel`

## Development Setup

1. Fork the repo and create your branch from `main`.
2. Install Python 3.10+ and Poetry.
3. Run the following commands:

```bash
# Clone your fork
git clone https://github.com/your-username/cortical-language-model.git
cd cortical-language-model

# Install dependencies
poetry install

# Set up pre-commit hooks
poetry run pre-commit install

# Run tests to make sure everything works
poetry run pytest
