# ✨ Contributing

Thank you for your interest in contributing to our projects! Contributions of all kinds are welcome, whether they involve fixing bugs, adding features, improving documentation, or enhancing code quality. This guide outlines the process for contributing and ensures consistency across all repositories under this organization.  

## Table of Contents  
1. [Code of Conduct](#code-of-conduct)  
2. [How Can I Contribute?](#how-can-i-contribute)  
   - [Reporting Issues](#reporting-issues)  
   - [Submitting Pull Requests](#submitting-pull-requests)  
   - [Proposing Features](#proposing-features)  
3. [Development Setup](#development-setup)  
4. [Coding Guidelines](#coding-guidelines)  
   - [General Practices](#general-practices)  
   - [Language-Specific Guidelines](#language-specific-guidelines)  
5. [Code Quality](#code-quality)  
6. [Breaking Changes](#breaking-changes)  
7. [Documentation](#documentation)  
8. [After Your Pull Request is Merged](#after-your-pull-request-is-merged)  

## 🤝 Code of Conduct  
By participating in this organization, you agree to uphold our [Code of Conduct](CODE_OF_CONDUCT.md). Please treat everyone respectfully and foster an inclusive, welcoming environment.  

## 💡 How Can I Contribute?  

### 🐛 Reporting Issues  
If you encounter a bug or have a suggestion:  
1. Check the [issue tracker](../../issues) for duplicates.  
2. If no similar issue exists, open a new issue and include:  
   - A descriptive title.  
   - Detailed information about the bug, feature, or suggestion.  
   - Steps to reproduce (if reporting a bug).  

### 🔄 Submitting Pull Requests  
1. Fork the repository and clone it locally.  
2. Create a branch for your changes:  
   ```bash
   git checkout -b feature/your-feature-name
   ```  
3. Make your changes and commit them with clear, concise messages.  
4. Push the branch to your fork:  
   ```bash
   git push origin feature/your-feature-name
   ```  
5. Submit a pull request to the `main` or appropriate branch of the repository.  

Ensure that your pull request:  
- Follows the [coding guidelines](#coding-guidelines).  
- Includes tests for new functionality, if applicable.  
- References related issues in the description (e.g., "Fixes #123").  

### 💭 Proposing Features  
If you’re considering a significant new feature, open an issue or discussion first to gather feedback and align with project goals.  

## 🛠️ Development Setup  
Refer to the specific repository’s `README.md` or `DEVELOPMENT.md` for setup instructions. Each project may use different dependencies or build tools, such as:  
- **Node.js**: Use `npm` or `yarn` to install dependencies.  
- **Python**: Set up a virtual environment and use `pip` for dependencies.  
- **Go**: Use `go mod` for dependency management.  
- **Rust**: Use `cargo` for building and testing.  
- **PHP**: Use `composer` for dependency management.  
- **C#**: Use `dotnet` CLI for building and testing.  

## 🧑‍💻 Coding Guidelines  

### 🌟 General Practices  
- Write clean, maintainable, and well-documented code.  
- Use meaningful names for variables, methods, and classes.  
- Include comments where necessary to explain complex logic.  
- Avoid introducing breaking changes unless absolutely necessary.  

### 📚 Language-Specific Guidelines  

#### C#  
- Follow [Microsoft’s C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions).  
- Use `async/await` for asynchronous operations.  

#### PHP  
- Follow [PSR-12](https://www.php-fig.org/psr/psr-12/) coding standards.  

#### Node.js / JavaScript / TypeScript  
- Use [ESLint](https://eslint.org/) for linting and code quality.  
- Follow [Airbnb's JavaScript Style Guide](https://github.com/airbnb/javascript) or the project’s established rules.  

#### Rust  
- Follow the [Rust API Guidelines](https://rust-lang.github.io/api-guidelines/).  
- Use `clippy` for linting and code quality checks.  

#### React  
- Use functional components and hooks.  
- Adhere to the [React Docs](https://reactjs.org/docs/getting-started.html) guidelines.  

#### Python  
- Follow [PEP 8](https://peps.python.org/pep-0008/) for coding style.  
- Use `flake8` or `black` for linting and formatting.  

#### Go  
- Follow [Effective Go](https://go.dev/doc/effective_go).  
- Use `golangci-lint` for static code analysis.  

## ✅ Code Quality  
All repositories prioritize code quality. Contributions should:  
- Include tests for new functionality (unit, integration, or end-to-end as applicable).  
- Pass all existing tests.  
- Use language-specific tools for static analysis and linting (e.g., `dotnet analyzers`, `flake8`, `eslint`, `clippy`, `golangci-lint`).  

## 🔥 Breaking Changes  
If your changes introduce breaking changes, you must ensure versioning is correctly updated to reflect the new major version. Follow these steps depending on the CI platform used by the project:  

### 🛠️ For Projects Using AppVeyor  
- Update the `appveyor.yml` file located at the root level of the repository to reflect the new major version.  
- Ensure that the semantic versioning aligns with the changes being introduced.  

### 🚀 For Projects Using GitHub Actions  
- Check if the project uses **GitVersion** to manage semantic versioning.  
- If GitVersion is being used:  
  - Include `+semver: major` in the commit message and pull request title to increment the version to the next major version automatically.  
  - Example commit message:  
    ```text
    Refactor API endpoint handling +semver: major  
    ```  
- If GitVersion is not used, consult the repository maintainers or refer to the project’s specific versioning process to determine the appropriate steps.  

### 📋 General Requirements  
- Clearly document the breaking changes in the pull request description.  
- Include any necessary migration steps or guidelines for users to adapt to the changes.  

## 📝 Documentation  
Please ensure that any changes to the code are reflected in the documentation:  
- Update the `docs` directory with any new, removed, or modified functionality.  
- If there are no public API changes, an update to the documentation may not be necessary.  

## 🎉 After Your Pull Request is Merged  
Once your pull request is merged:  
- You can safely delete your branch from your forked repository.
