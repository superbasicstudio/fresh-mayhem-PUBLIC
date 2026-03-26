# Fresh Mayhem — Downloads

**Desktop companion app for HackRF One and PortaPack devices.**

Compatible with HackRF One, PortaPack H4M (Mayhem firmware), and potentially other HackRF-compatible devices.

> Fresh Mayhem is not affiliated with, endorsed by, or sponsored by Great Scott Gadgets, Sharebrained Technology, or any hardware manufacturer. HackRF, HackRF One, and PortaPack are trademarks of their respective owners.

---

## Downloads

Download the latest release for your platform from the [Releases](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/releases) page.

### Linux
| Format | Description |
|--------|-------------|
| `.deb` | Debian, Ubuntu, Pop!_OS, Linux Mint |
| `.rpm` | Fedora, openSUSE, CentOS, RHEL |
| `.AppImage` | Universal — runs on any distro (coming soon) |

### macOS
| Format | Description |
|--------|-------------|
| `.dmg` | macOS 11+ (Intel and Apple Silicon) — coming soon |

### Windows
| Format | Description |
|--------|-------------|
| `.msi` | Windows 10/11 installer — coming soon |

---

## Verify Downloads

Each release includes SHA-256 checksums. To verify:

```bash
# Linux/macOS
sha256sum FreshMayhem_*.deb

# Windows (PowerShell)
Get-FileHash FreshMayhem_*.msi -Algorithm SHA256
```

Compare the output against the checksums listed in the release notes.

---

## Requirements

- **HackRF tools** installed (`hackrf_info`, `hackrf_transfer`, `hackrf_sweep`)
- **Ollama** (optional) — for natural language commands. Download at [ollama.com](https://ollama.com)
- **USB data cable** (not a charging-only cable)

---

## Links

- [Website](https://freshmayhem.com)
- [Report Issues](https://github.com/superbasicstudio/fresh-mayhem-PUBLIC/issues)

---

**Proprietary software by [Super Basic Studio, LLC](https://superbasic.studio)**
Free during beta (v0.8.x). See LICENSE for terms.
