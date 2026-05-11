<h1 align="center">🖥️ Scribtly Desktop</h1>

<p align="center">
  <strong>Open-source desktop companion for <a href="https://scribtly.com">scribtly.com</a> — AI script generator that runs 100% locally</strong>
</p>

<p align="center">
  <a href="https://scribtly.com"><img src="https://img.shields.io/badge/🌐_scribtly.com-web%20app-2563eb?style=flat-square" alt="scribtly.com"></a>
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=flat-square">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square">
  <img src="https://img.shields.io/badge/Status-In%20Development-orange?style=flat-square">
  <img src="https://img.shields.io/badge/Price-Free-brightgreen?style=flat-square">
  <img src="https://img.shields.io/badge/Open%20Source-%E2%9D%A4-red?style=flat-square">
</p>

<p align="center">
  <strong><a href="https://scribtly.com">→ Try Scribtly on the web at scribtly.com</a></strong>
</p>

---

## ✨ What is Scribtly Desktop?

Scribtly Desktop is the open-source, offline-first desktop companion to [scribtly.com](https://scribtly.com) — the AI script generator for content creators. Same powerful script generation, but it runs entirely on your machine. No subscriptions. No cloud. No data leaves your device.

**Bring your own API key. Your scripts stay yours.**

## 🔥 Features

- **🎬 Script Generator** — Pick platform, hook style, tone, length — AI writes platform-specific scripts
- **📚 Local Script Library** — Browse, search, and manage scripts in a local SQLite database
- **🗺 Roadmap Planner** — Plan content topics, set goals, and visualise your schedule
- **⚙️ Bring Your Own Key** — OpenAI GPT or Anthropic Claude — your key, stored locally only
- **📄 PDF Export** — Export any script for sharing or printing
- **🔒 100% Private** — No telemetry, no analytics, no servers. Ever.

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Language | Python 3.10+ |
| UI | Tkinter |
| Database | SQLite3 (local) |
| AI | OpenAI GPT · Anthropic Claude |
| Charts | Matplotlib |
| PDF Export | ReportLab |
| Architecture | OOP |

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- An [OpenAI](https://platform.openai.com) or [Anthropic](https://console.anthropic.com) API key

### Install & Run

```bash
git clone https://github.com/tsvtnv/Scribtly-Desktop.git
cd Scribtly-Desktop
pip install -r requirements.txt
python main.py
```

### API Key Setup

Open **Settings** in the app and paste your API key. It is stored locally on your device only — never sent anywhere except the AI provider you chose.

## 🗓 Roadmap

- [x] Project architecture & database schema
- [ ] Tkinter UI shell
- [ ] Script generator core (platform, tone, hook, style)
- [ ] Local script library with search
- [ ] PDF export
- [ ] Content roadmap planner
- [ ] Packaged installer (`.exe` / `.app` / `.AppImage`)
- [ ] Offline model support (no API key required)

## 🌐 Scribtly Web vs Desktop

| Feature | [scribtly.com](https://scribtly.com) | Scribtly Desktop |
|---------|-------------|------------------|
| Hosting | Cloud (we run it) | Your machine |
| API key | Managed for you | Bring your own |
| Subscription | Yes | Free forever |
| Privacy | Standard SaaS | 100% local |
| Offline use | No | Yes |

## 🤝 Contributing

Contributions welcome — this is community open source.

1. Fork the repo
2. Create a branch: `git checkout -b feat/your-feature`
3. Commit: `git commit -m "feat: add your feature"`
4. Push and open a Pull Request

## 🔒 Privacy

All scripts and user data are stored in a local SQLite database. No analytics, no telemetry, no external servers — ever. The only network call is to your chosen AI provider (OpenAI or Anthropic) when you generate a script.

## 📄 License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE).

---

<p align="center">
  Made by <a href="https://tsvweb.com"><strong>tsvweb.com</strong></a> · Birmingham, UK 🇬🇧<br>
  <a href="https://scribtly.com">scribtly.com</a> · the cloud version
</p>