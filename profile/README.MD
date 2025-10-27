# Watchiko

**Watchiko** is an activity monitoring and reporting system designed for personally-owned computer systems. It helps users gain insight into their own system usage patterns, device events, and local activity — all while respecting privacy and ethical boundaries.

---

## 🧩 System Overview

Watchiko is built as a modular four-tier system:

- **Daemon**: A background service that monitors system-level events
- **Repository**: Local storage for event logs and activity data
- **Client**: A user-facing interface or API for viewing and interacting with logs
- **Communication Channels**: Mechanisms for syncing data and reporting activity to cloud services

---

## ⚠️ Ethical Usage Warning

Watchiko is **not** spyware. It is **not** intended for surveillance or unauthorized monitoring of other users. The software must only be installed and used on systems **personally owned and operated** by the user.

### ❌ Watchiko does **not** support:
- Recording webcam feeds
- Capturing audio sources
- Taking random screenshots
- Streaming live screencasts

These features are **explicitly excluded** from Watchiko’s design and purpose.

### ✅ Watchiko is intended **only** for:
- Monitoring your own device activity
- Tracking system events (e.g., USB insert/remove)
- Logging and analyzing usage patterns on your personal machine

---

## 📜 Legal Disclaimer

By installing and using Watchiko, you acknowledge and agree to the following:

- You will use Watchiko **only** on systems you personally own and operate.
- You will **not** use Watchiko to monitor other individuals without their knowledge or consent.
- You understand that misuse of this software may violate local laws and regulations.
- You accept full responsibility for how Watchiko is used on your system.

---

## 🧠 Philosophy

Watchiko is built with a strong emphasis on:

- **Transparency**: Users know exactly what is being tracked
- **Modularity**: Event tracking is plugin-based and user-configurable
- **Security**: Core features like cloud sync and reporting are non-optional and tightly controlled
- **Privacy**: No invasive features, no hidden surveillance

---

## 🚀 Getting Started

To begin using Watchiko:

1. Install the software on your personal machine
2. Enable the plugins for the events you want to track (e.g., USB activity)
3. View logs and reports via the client interface
4. Sync data securely to your cloud dashboard (optional)

---

## 📂 Plugin Architecture

Watchiko supports a hybrid plugin system:

- Each plugin contains:
  - `plugin.ts`: High-level orchestration logic
  - `plugin.go`: Native system hook implementation (optional)
- Users can author their own plugins using the provided template
- Plugins are loaded dynamically and can be enabled/disabled independently

---

## 📬 Contact & Contributions

Watchiko is an open project. Contributions, feedback, and responsible usage are welcome.

---

