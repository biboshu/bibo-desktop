<p align="center">
  <img src="src-tauri/icons/128x128.png" alt="Bibo Logo" width="80" />
</p>

<h1 align="center">Bibo</h1>

<p align="center">
  A lightweight, open-source note-taking app inspired by Notion.
</p>

<p align="center">
  <a href="https://github.com/biboshu/bibo-desktop/releases"><img src="https://img.shields.io/github/v/release/biboshu/bibo-desktop" alt="Latest Release"></a>
  <a href="https://github.com/biboshu/bibo-desktop/blob/main/LICENSE"><img src="https://img.shields.io/github/license/biboshu/bibo-desktop" alt="License"></a>
  <a href="https://github.com/biboshu/bibo-desktop/releases"><img src="https://img.shields.io/github/downloads/biboshu/bibo-desktop/total" alt="Downloads"></a>
</p>

## About Bibo

> **Note:** This repository contains the Tauri desktop shell for Bibo. The frontend webapp lives in a separate repository: [biboshu/bibo-webapp](https://github.com/biboshu/bibo-webapp).

Bibo is a note-taking desktop application that aims to provide a Notion-like experience while staying **lightweight** and **open source**. Built with Tauri and SvelteKit for a fast, native feel with minimal resource usage.

- 📝 Block-based editor
- 🪶 Lightweight — minimal memory and disk footprint
- 🔒 Privacy-first — your notes stay yours
- 🔄 Auto-updates
- 🐧🪟🍎 Cross-platform (Linux, Windows, macOS)

## Local Development

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS)
- [pnpm](https://pnpm.io/)
- [Rust](https://www.rust-lang.org/tools/install)
- Tauri system dependencies ([see docs](https://v2.tauri.app/start/prerequisites/))

### Setup

This project requires the [bibo-webapp](https://github.com/biboshu/bibo-webapp) repository to be cloned alongside this one:

```bash
mkdir bibo && cd bibo
git clone https://github.com/biboshu/bibo-webapp.git webapp
git clone https://github.com/biboshu/bibo-desktop.git client
```

Your directory structure should look like this:

```
bibo/
├── webapp/    # Frontend (SvelteKit)
└── client/    # Desktop shell (Tauri)
```

Then install dependencies and run:

```bash
cd webapp
pnpm install

cd ../client
pnpm install
pnpm tauri:dev
```

## Contributing

Thank you for considering contributing to Bibo! Please read the [contribution guide](CONTRIBUTING.md) before submitting a pull request.

## Code of Conduct

Please review and abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Security Vulnerabilities

If you discover a security vulnerability, please send an email to the maintainers. All security vulnerabilities will be promptly addressed.

## License

Bibo is open-source software licensed under the [AGPL-3.0-or-later](LICENSE) license.
