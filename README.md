# Fresh Mayhem

**Desktop companion app compatible with HackRF One and PortaPack devices.**

Natural language SDR control, frequency sweeps, signal capture, spectrum visualization, and an embedded RF knowledge base. Works with or without an LLM.

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

- **Natural language device control** — "capture 433 MHz", "full spectrum sweep", "sweep the WiFi band"
- **Capture and analyze** — IQ raw, WAV, and sweep CSV files saved locally
- **Loot file analysis** — click CHAT on any capture and get peak frequencies, signal identification, noise floor stats
- **In-app spectrum viewer** — visualize sweep data without leaving the app
- **Device health check** — read-only hardware diagnostics (clock synth, mixer, transceiver, M0 state)
- **28 FAQs with search** — troubleshooting for Linux, macOS, Windows, device setup, LLM models
- **50 "Did You Know" tips** — RF fundamentals, signal hunting, PortaPack tricks
- **15 languages** — full i18n across all features
- **Works without LLM** — MANUAL mode for direct CLI commands, no Ollama required
- **Privacy-first** — all data stays local, no telemetry, no tracking

---

## Supported Commands

The app wraps the standard HackRF CLI tools. Anything you can do with hackrf_transfer or hackrf_sweep, you can do here. The intent parser understands ~50 natural language patterns:

### Frequency Captures
- `capture 433 MHz` / `capture 868 MHz` / `capture 915 MHz` (ISM bands)
- `capture 1090 MHz` (ADS-B aircraft tracking)
- `capture 162.4 MHz` (NOAA weather radio)
- `capture 152 MHz` (pager/POCSAG)
- `capture [any frequency]` with MHz, GHz, kHz, or Hz

### Frequency Sweeps
- `full spectrum sweep` (0-6 GHz)
- `sweep 400 to 500 MHz` (custom range)
- `sweep FM band` (88-108 MHz)
- `sweep WiFi band` (2.4 GHz or 5 GHz)

### Protocol/Band Shortcuts
- `scan WiFi` / `scan Bluetooth` / `scan LoRa`
- `listen for ADS-B` / `listen for GPS`
- `capture TPMS` / `capture marine AIS`
- `scan amateur 2m band` / `scan 70cm band`

### Device Control
- `set LNA gain to 24` / `set VGA gain to 30` / `set TX gain to 20`
- `amp on` / `amp off` / `bias tee on` / `bias tee off`
- `device info` / `firmware version`
- `list my captures` / `stop`

### Duration Support
- `capture 433 MHz for 2 minutes`
- `sweep 400 to 500 for 30 seconds`

### Questions (routed to LLM with RF knowledge base)
- `what is OOK modulation?`
- `what frequency do garage doors use?`
- `explain the difference between AM and FM`

Anything the parser doesn't recognize gets passed to the LLM, which can call all of the same tools. There's also MANUAL mode for typing raw hackrf CLI commands directly.

---

## Compatible Devices

| Device | Status |
|--------|--------|
| HackRF One | Fully supported |
| PortaPack H4M (Mayhem firmware) | Supported (limited mode) |
| HackRF One Pro | Should work, untested |
| Older PortaPacks (H1/H2/H2+) | May work with Mayhem firmware, untested |

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

## Third-Party Licenses

All dependencies use permissive licenses (MIT, Apache-2.0, ISC, BSD-3-Clause, MPL-2.0 file-level). No GPL code is included in the application.

HackRF CLI tools (hackrf_info, hackrf_transfer, hackrf_sweep, etc.) are GPLv2 and developed by Great Scott Gadgets. They are called as separate external processes, not bundled or linked into this application. Users install them independently.

A full dependency audit (324 crates and packages) is maintained in the source repository.

---

## Issues & Feedback

Found a bug or have a feature request? **[Open an issue](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/issues/new/choose)**.

Please include:
- Your platform (Linux distro, macOS version, etc.)
- App version (shown in the BETA badge)
- Device type (HackRF One, PortaPack, etc.)
- Steps to reproduce

Check the in-app **FAQ tab** (question mark icon) before submitting. Many common issues are covered there.

New to GitHub issues? See our [step-by-step guide](SUPPORT.md).

---

## Links

- [Download Page](https://www.superbasic.studio/software/fresh-mayhem)
- [Website](https://freshmayhem.com)
- [Super Basic Studio](https://superbasic.studio)

---

**Proprietary software by [Super Basic Studio, LLC](https://superbasic.studio)** — Free during beta.
