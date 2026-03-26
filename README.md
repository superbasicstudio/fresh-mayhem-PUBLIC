# Fresh Mayhem

**Desktop companion app compatible with HackRF One and PortaPack devices.**

Natural language SDR control, frequency sweeps, signal capture, spectrum visualization, and an embedded RF knowledge base — all in one app. Works with or without an LLM.

> Fresh Mayhem is not affiliated with, endorsed by, or sponsored by Great Scott Gadgets, Sharebrained Technology, or any hardware manufacturer. HackRF, HackRF One, and PortaPack are trademarks of their respective owners.

---

## Downloads

Download the latest release for your platform from the **[Releases](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/releases)** page.

### Linux (Available Now)
| Format | Best For |
|--------|----------|
| `.deb` | Debian, Ubuntu, Pop!_OS, Linux Mint |
| `.rpm` | Fedora, openSUSE, CentOS, RHEL |
| `.AppImage` | Any distro (universal, no install needed) |

### macOS — Coming Soon
Signed and notarized DMG for macOS 11+ (Intel and Apple Silicon). Currently in testing.

### Windows — Coming Soon
MSI installer for Windows 10/11. Currently in development.

---

## What It Does

- **Natural language device control** — "capture 433 MHz", "full spectrum sweep", "listen on 1090 for ADS-B"
- **Capture & analyze** — IQ raw, WAV, and sweep CSV files saved locally
- **In-app spectrum viewer** — visualize sweep data without leaving the app
- **28 FAQs with search** — troubleshooting for Linux, macOS, Windows, device setup
- **50 "Did You Know" tips** — RF fundamentals, signal hunting, PortaPack tricks
- **15 languages** — full i18n across all features
- **Works without LLM** — ADVANCED mode for direct CLI commands, no Ollama required
- **Privacy-first** — all data stays local, no telemetry, no tracking

## Compatible Devices

| Device | Status |
|--------|--------|
| HackRF One | Fully supported |
| PortaPack H4M (Mayhem firmware) | Supported (limited mode) |
| HackRF One Pro | Should work — untested |
| Older PortaPacks (H1/H2/H2+) | May work with Mayhem firmware — untested |

---

## Quick Start

1. **Install HackRF tools** — `sudo apt install hackrf` (Debian/Ubuntu) or equivalent
2. **Connect your HackRF** via USB data cable (not charging-only)
3. **Install Fresh Mayhem** — download .deb/.rpm/.AppImage from [Releases](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/releases)
4. **Optional: Install Ollama** for natural language commands — [ollama.com](https://ollama.com)
5. **Launch** and click the FRESH MAYHEM logo to scan for your device

---

## Verify Downloads

Each release includes SHA-256 checksums in the release notes.

```bash
sha256sum Fresh\ Mayhem_*.deb
```

---

## Issues & Feedback

Found a bug or have a feature request? **[Open an issue](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/issues/new/choose)**.

Please include:
- Your platform (Linux distro, macOS version, etc.)
- App version (shown in the BETA badge)
- Device type (HackRF One, PortaPack, etc.)
- Steps to reproduce

Check the in-app **FAQ tab** (question mark icon) before submitting — many common issues are covered there.

---

## Links

- [Website](https://freshmayhem.com)
- [Super Basic Studio](https://superbasic.studio)

---

**Proprietary software by [Super Basic Studio, LLC](https://superbasic.studio)** — Free during beta.
