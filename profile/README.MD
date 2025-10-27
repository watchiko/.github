# Watchiko

**Watchiko** is a real-time activity monitoring and reporting system designed for personally-owned computer systems. It helps users gain insight into their own system usage patterns, device events, and local activity — all while respecting privacy and ethical boundaries.

---

## 🎯 Purpose

Watchiko is built for **personal digital forensics** with a **live-first mindset**. It doesn’t just log what happened — it alerts you **as soon as something happens**.

Whether it’s a USB device being plugged in, a suspicious process starting, or a file being transferred, Watchiko is designed to:

- **Detect** events immediately
- **Classify** them based on severity
- **Report** them to you or your cloud dashboard
- **Store** them for later analysis

It’s like a personal black box for your system — but one that speaks up the moment something matters.

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
- **Modularity**: Event tracking is defined through composable event hooks and optional native implementations
- **Security**: Core features like cloud sync and reporting are non-optional and tightly controlled
- **Privacy**: No invasive features, no hidden surveillance
- **Forensic Value**: Every event is timestamped, classified, and stored for later review
- **Live-ness**: Alerts are generated **as soon as** events are detected — not hours later

---

## 📂 Event Hook Architecture

Watchiko supports a hybrid event hook system:

- Each **event hook module** consists of:
  - `hook.ts`: High-level orchestration logic that defines what to track and how to respond
  - `hook.go`: Optional native implementation for system-level access (e.g., USB detection)
- These modules are stored in the `event-hooks/` folder
- Users can author their own hooks using the provided template
- Hooks are dynamically loaded and can be enabled/disabled independently

---

## 🚀 Getting Started

To begin using Watchiko:

1. Install the software on your personal machine
2. Enable the event hooks for the activities you want to track (e.g., USB activity)
3. View logs and reports via the client interface
4. Sync data securely to your cloud dashboard (optional)

---

## 📬 Contact & Contributions

Watchiko is an open project. Contributions, feedback, and responsible usage are welcome.

---
