# VOID

> Where your ideas live.

VOID is a personal productivity and academic management app for Android. Built for university life — notes, habits, exams, schedules, and an AI assistant, all in one place. Offline-first, encrypted, no accounts required.

---

## The App

VOID started as a personal tool and grew into something more complete. It's designed around the idea that your productivity system should understand your academic context — not just store files, but know that a note belongs to a subject, that a subject has exams, and that those exams have dates.

**Core features:**

- **Block editor** — Notion-style live preview with 12 block types, slash commands, drag-and-drop, and full Markdown support
- **Handwritten notebooks** — Vector-based drawing canvas with pressure sensitivity, multi-page support, dot grid, and ruled backgrounds
- **AI assistant** — Local Ollama or cloud models (Gemini, OpenAI, Anthropic, OpenRouter) with full tool calling and 11 tools
- **Academic management** — Subjects, exams, attendance tracking, and schedules; all linked to your notes
- **Habits & Pomodoro** — Build routines, track streaks, and stay focused
- **Publish to web** — Push notes to a personal GitHub Pages site with one tap; version history included
- **P2P sync** — End-to-end encrypted local network sync, no cloud required

---

## Repositories

| Repo | Description |
|---|---|
| [`void-android`](https://github.com/welcomethevoid/void-android) | Main Android app — Kotlin, Jetpack Compose, Room, Hilt |
| [`void-pages`](https://github.com/welcomethevoid/void-pages) | Static site engine for published notes |
| [`void-landing`](https://github.com/welcomethevoid/void-landing) | Landing page — [welcomethevoid.github.io/void-landing](https://welcomethevoid.github.io/void-landing) |

Each user's published notes live in their own `void-notes` repo, created automatically by the app when they connect GitHub.

---

## Tech Stack

**Android**
- Kotlin · Jetpack Compose · Room · Hilt · WorkManager
- Navigation Compose · Glance (widgets) · DataStore

**Sync**
- Custom UDP broadcast · ECDH key exchange · AES-256-GCM encryption
- mDNS device discovery via `NsdManager` · Last-write-wins conflict resolution

**AI**
- Ollama (local) · Gemini · OpenAI · Anthropic · OpenRouter
- Full tool calling with 11 tools · Intelligent tool routing · 16,384 token context

**Publishing**
- JGit · GitHub OAuth Device Flow · GitHub Actions · GitHub Pages
- `void-pages` static site generator (Node.js · marked)

**Design system**
- Pure `#000000` AMOLED backgrounds · Zero border radius · Zero elevation
- Big Shoulders Display · JetBrains Mono · `#A8B0BC` Plata Frío accent
- 36-tone muted palette · Grid background texture · Radial glow on key numbers

---

## Project Status

VOID is in active development, approaching its first release. It is currently a personal-use app — not yet available on the Play Store. APK releases will be published here when ready.

---

## Contributing

VOID is primarily a personal project. That said, if you find a bug, have a suggestion, or want to contribute, feel free to open an issue in the relevant repository.

---

## License

To be defined before public release.

---

*Built by [@Pebrd](https://github.com/Pebrd) · Buenos Aires, Argentina*
