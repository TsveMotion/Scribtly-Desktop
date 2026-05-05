# Scribtly Desktop

**AI Script Generator for Social Media Influencers — Desktop App**

> **Status: Idea / Pre-development**
> This project is currently in the planning stage as part of a Component 3 OCR Computer Science A-Level project.

Inspired by [Scribtly.com](https://scribtly.com), Scribtly Desktop is a planned free and open-source desktop application that will help content creators generate high-quality scripts for social media platforms. Everything will run locally with no servers, no subscriptions, and no data ever leaving your machine.

---

## Free & Open Source

Scribtly Desktop is **100% free** and released under the **MIT License**. You are free to use, modify, and distribute it for any purpose. See [LICENSE](LICENSE) for full details.

---

## Features

- **Home**: Welcome dashboard with quick-start overview
- **Generate**: Create scripts by specifying platform, hooks, tone, and style using AI (OpenAI GPT or Anthropic Claude Sonnet)
- **Library**: Browse, search, and manage all your saved scripts locally
- **Roadmaps** *(Extension)*: Plan topics, set content goals, and visualise your progress
- **Settings**: Configure your API key and personal preferences

---

## Tech Stack

| Layer | Technology |
|---|---|
| UI | Tkinter |
| Database | SQLite3 (local, no cloud) |
| AI | OpenAI GPT / Anthropic Claude Sonnet |
| Charts | Matplotlib |
| Pathfinding | Dijkstra's Algorithm |
| PDF Export | ReportLab |
| Architecture | OOP (Python) |

---

## Getting Started

### Prerequisites

- Python 3.10+
- An OpenAI or Anthropic API key

### Installation

```bash
git clone https://github.com/TsveMotion/scribtly-desktop.git
cd scribtly-desktop
pip install -r requirements.txt
python main.py
```

### API Key Setup

Open **Settings** inside the app and paste your API key. It is stored locally on your device only.

---

## Privacy

All scripts and user data are stored in a local SQLite database on your machine. No analytics, no telemetry, no external servers.

---

## License

MIT License. Copyright (c) 2026 Kristiyan Tsvetanov. See [LICENSE](LICENSE).
