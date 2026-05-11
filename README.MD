<h1 align="center">
  <img src="https://img.shields.io/badge/Scribtly-Desktop-2563eb?style=for-the-badge&logo=python&logoColor=white" alt="Scribtly Desktop">
</h1>

<h3 align="center">AI-powered script generator for content creators — runs 100% on your machine</h3>

<p align="center">
  <a href="https://scribtly.com"><img src="https://img.shields.io/badge/🌐_scribtly.com-live-2563eb?style=flat-square" alt="scribtly.com"></a>
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/License-MIT-yellow?style=flat-square">
  <img src="https://img.shields.io/badge/Status-In%20Development-orange?style=flat-square">
  <img src="https://img.shields.io/badge/Price-Free-brightgreen?style=flat-square">
</p>

<p align="center">
  <strong><a href="https://scribtly.com">Try the web app → scribtly.com</a></strong>
</p>

---

## What is Scribtly Desktop?

Scribtly Desktop is the offline, open-source companion to [scribtly.com](https://scribtly.com) — a tool that helps content creators generate high-quality, platform-specific scripts for YouTube, TikTok, Instagram Reels, and more.

Everything runs **locally on your machine**. No subscriptions. No cloud. No data ever leaves your device. Just bring your own API key.

---

## ✨ Features

- **🎬 Script Generator** — Specify platform, hook style, tone, and length. AI writes the script.
- **📚 Script Library** — Browse, search, and manage all your saved scripts locally with SQLite.
- **🗺 Roadmap Planner** *(extension)* — Plan content topics, set goals, and visualise your schedule.
- **⚙️ Settings** — Configure your API key (OpenAI or Anthropic Claude) once. Stored locally only.
- **📄 PDF Export** — Export any script to PDF for sharing or printing.
- **🔒 100% Private** — No telemetry, no analytics, no external servers. Your scripts stay yours.

---

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

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- An [OpenAI](https://platform.openai.com) or [Anthropic](https://console.anthropic.com) API key

### Install & Run

```bash
git clone https://github.com/tsvtnv/Scribtly.git
cd Scribtly
pip install -r requirements.txt
python main.py
```

### API Key Setup

Open **Settings** inside the app and paste your API key. Stored locally only — never sent anywhere else.

---

## 🗓 Roadmap

- [x] Project architecture & database schema
- [x] Script generator core (platform, tone, hook, style)
- [x] Local script library with search
- [ ] PDF export
- [ ] Content roadmap planner
- [ ] Packaged installer (Windows `.exe` / macOS `.app`)
- [ ] Offline model support (no API key required)

---

## 🤝 Contributing

1. Fork the repo
2. Create a branch: `git checkout -b feat/your-feature`
3. Commit: `git commit -m 'feat: add your feature'`
4. Push and open a Pull Request

---

## 🔒 Privacy

All scripts and data are stored in a local SQLite database. No analytics, no telemetry, no external servers — ever.

---

## 📄 License

MIT — free to use, modify, and distribute. See [LICENSE](LICENSE).

---

<p align="center">
  Built by <a href="https://tsvweb.com"><strong>TsvWeb</strong></a> · Birmingham, UK 🇬🇧<br>
  <a href="https://scribtly.com">scribtly.com</a>
</p>