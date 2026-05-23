# Content Coach - Public Releases

This repository hosts the public releases for Content Coach, a desktop application for TCGplayer employees to write on-brand communications using AI.

## 🚀 Quick Install

```bash
curl -fsSL https://raw.githubusercontent.com/TCGplayer/Electron-Content-Coach-Releases/main/install.sh | bash
```

## 📱 What is Content Coach?

Content Coach helps TCGplayer employees write communications that align with our brand voice and guidelines. Built with Electron, Next.js, and React Spring, it combines a modern UI with AI-powered content correction and generation.

### ✨ Features

- **Improve Text** — Paste existing copy and get an on-brand revision with rationale
- **Create Content** — Describe what you need and generate brand-aligned copy from scratch
- **Design Link** — Paste a Figma URL to generate all copy for a screen at once
- **Component-aware** — Knows the format rules for errors, alerts, CTAs, headings, helper text, and more
- **RAG-powered guidelines** — Retrieves the most relevant brand guidelines for each request
- **Refinement actions** — Simplify, shorten, clarify, or apply a custom instruction to any result
- **Variant tabs** — Get 3 alternative versions with every response
- **Atlassian context** — Optionally pull in Jira/Confluence project context to align terminology
- **Automatic Updates** — The app notifies you when a new version is available

## 🎨 Built With

- **Electron** — Cross-platform desktop framework
- **Next.js** — React framework for the UI
- **React Spring** — Smooth animations and transitions
- **PyChomsky** — eBay's internal AI SDK for LLM calls and embeddings
- **Claude Sonnet** — Primary model for tone correction and content generation
- **Local vector index** — Bundled guideline embeddings, no external database required
- **FontAwesome** — Icons throughout the app

## 🔄 Automatic Updates

Content Coach checks for new versions on launch and shows a banner when one is available. Updates are manual installs (re-run the installer or download the DMG from the Releases page).

## 📥 Manual Installation

1. Download the latest `Content-Coach-X.X.X-arm64.dmg` from the [Releases page](https://github.com/TCGplayer/Electron-Content-Coach-Releases/releases)
2. Open the DMG and drag **Content Coach** to your Applications folder
3. Right-click the app and select **Open** on first launch (to bypass macOS Gatekeeper)

## 🏠 Source Code

The source code lives in the private repository for TCGplayer employees: [TCGplayer/Electron_Content_Coach](https://github.com/TCGplayer/Electron_Content_Coach)

## 🆘 Support

For issues or questions, open an issue in the main source repository or contact the development team.

---

**Built with ❤️ for TCGplayer**
