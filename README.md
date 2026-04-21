# ⚙️ Dotfiles Manager CLI

<div align="center">
  <img src="https://img.shields.io/badge/Language-Go-blue.svg" alt="Language Go" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License MIT" />
  <p><strong>A fast, cross-platform CLI for managing, syncing, and encrypting your dotfiles.</strong></p>
</div>

## ✨ Overview

Every developer eventually struggles with keeping their terminal environment, aliases, and specific tool configurations synchronized across multiple machines. **Dotfiles Manager** is a zero-dependency (written in Go) CLI utility designed to eliminate this friction entirely.

Instead of writing complex bash setup scripts or relying on GNU Stow, this tool explicitly manages symlinks, encrypts sensitive API keys, and tracks multiple "profiles" (e.g., Work vs. Personal) seamlessly.

## 🚀 Key Features

- **Profile Switching**: Keep `.gitconfig-work` distinct from `.gitconfig-personal`. Switch with a single command.
- **Native Encryption**: Transparently encrypt sensitive files (like `.npmrc` with tokens) using AES-256 before pushing to your remote git repository.
- **1-Click Restore**: Boots up a fresh environment. Run `dot pull` and instantly have your preferred bash/zsh/fish environment working perfectly.
- **Cross-Platform**: Compiles to a single binary. Works on macOS, Linux, and Windows (WSL).

## 📦 Installation

```bash
curl -fsSL https://raw.githubusercontent.com/RanaAhmar/dotfiles-manager/main/install.sh | bash
```

## 💻 Quick Start

```bash
# Initialize tracking in your home directory
dot init ~/.dotfiles

# Track a specific config file
dot track ~/.zshrc

# Encrypt a file containing secrets
dot track ~/.aws/credentials --encrypt

# Push to your remote backup (runs git commit and push under the hood)
dot sync
```

## 🤝 Contributing

We welcome community pull requests! Specifically looking for expansion on the Windows PowerShell symlink support logic. Please read our `CONTRIBUTING.md` before submitting code.







---

## 🚀 Discover More from Stackaura

If you found this tool useful, check out our other high-performance web utilities and follow **Ahmar Hussain** for more open-source excellence.

### 🌟 Featured Projects
- **[Stackaura Hub](https://github.com/RanaAhmar/stackaura-hub)** - The central index for all 100 repositories.
- **[Free LLM APIs](https://github.com/RanaAhmar/free-llm-apis)** - A curated list of zero-cost AI endpoints.
- **[Awesome MCP Servers](https://github.com/RanaAhmar/awesome-mcp-servers)** - The ultimate collection of Model Context Protocol implementations.
- **[System Design Cheatsheet](https://github.com/RanaAhmar/system-design-cheatsheet)** - Master complex architectures in minutes.
- **[Next.js SaaS Starter](https://github.com/RanaAhmar/nextjs-saas-starter)** - The fastest way to launch your next product.

### 🔗 Stay Connected
- **Website:** [stackaura.com](https://www.stackaura.com/)
- **Author:** [Ahmar Hussain](https://github.com/RanaAhmar)

---






