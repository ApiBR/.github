# 🏛️ Organization-wide GitHub configuration

This repository acts as the **community health repository** for the organization. It provides **default templates and guidelines** that apply automatically across all repositories, unless specifically overridden. Its purpose is to enforce best practices, promote consistency, and streamline contribution workflows.

---

## 📦 Repository contents

### 1. Issue and pull request templates 📝
Standardized templates to guide contributors and maintain clean, useful conversations.

- `.github/ISSUE_TEMPLATE/bug_report.md` 🐛 – For reporting bugs
- `.github/ISSUE_TEMPLATE/feature_request.md` ✨ – For feature suggestions
- `.github/PULL_REQUEST_TEMPLATE.md` 🔄 – For submitting pull requests

### 2. Code of conduct 🤝  
Promotes a respectful and inclusive community across all organization projects.

- `CODE_OF_CONDUCT.md`

### 3. Contributing guidelines 📜  
Outlines how to contribute to organization repositories, including branch strategy and review processes.

- `CONTRIBUTING.md`

### 4. Security policy 🔒  
Describes how to report vulnerabilities securely and responsibly.

- `SECURITY.md`

---

## ⚙️ How it works

GitHub automatically applies the files from this `.github` repository to **all organization repositories** unless they include their own versions of the same files. This ensures every project starts with solid community and contribution standards.

---

## ✏️ Customization

To override or extend the defaults for a specific repository:
- Add your custom file (e.g. `CONTRIBUTING.md`, `ISSUE_TEMPLATE`) to that repository.
- GitHub will use the local version instead of the one in `.github`.

---

## 🤗 Contributing

We welcome improvements to these shared templates and guidelines!

1. Fork this repository.
2. Create a new branch for your changes.
3. Submit a pull request with a clear description of what you’re improving and why.

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE).

---

> ℹ️ For more details about GitHub community health files, check out the [official GitHub documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).
