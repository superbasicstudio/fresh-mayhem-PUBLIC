# Third-Party Licenses

Fresh Mayhem is proprietary software by Super Basic Studio, LLC. It incorporates the following open-source dependencies, all under permissive licenses that allow commercial use and proprietary distribution.

**No GPL or AGPL code is included in this application.** HackRF CLI tools (hackrf_info, hackrf_transfer, etc.) are GPLv2 but are called as separate external processes, not bundled, linked, or compiled into this application.

---

## License Summary

| License | Count | Type |
|---------|-------|------|
| MIT | 122 | Permissive |
| Apache-2.0 | 146 | Permissive |
| MIT OR Apache-2.0 | 14 | Permissive (dual-licensed) |
| Unicode-3.0 | 19 | Permissive (data) |
| MPL-2.0 | 5 | Weak copyleft (file-level only) |
| BSD-3-Clause | 4 | Permissive |
| ISC | 3 | Permissive |
| Unlicense | 2 | Public domain equivalent |
| BSL-1.0 (Boost) | 1 | Permissive |
| CDLA-Permissive-2.0 | 1 | Permissive (data) |
| Zlib | 1 | Permissive |

Total: ~324 transitive dependencies across the Rust and JavaScript stacks.

---

## Key Direct Dependencies

### Rust (Backend)

| Crate | License | Purpose |
|-------|---------|---------|
| tauri | Apache-2.0 OR MIT | Desktop app framework |
| tauri-plugin-shell | Apache-2.0 OR MIT | Process execution |
| tauri-plugin-window-state | Apache-2.0 OR MIT | Window position persistence |
| tokio | MIT | Async runtime |
| reqwest | MIT OR Apache-2.0 | HTTP client (Ollama/API) |
| serde / serde_json | MIT OR Apache-2.0 | Serialization |
| anyhow | MIT OR Apache-2.0 | Error handling |
| chrono | MIT OR Apache-2.0 | Date/time |
| regex | MIT OR Apache-2.0 | Pattern matching |
| sha2 / hex | MIT OR Apache-2.0 | Cryptographic hashing |
| dirs | MIT OR Apache-2.0 | Platform directory paths |
| sysinfo | MIT | System monitoring |
| uuid | Apache-2.0 OR MIT | Unique identifiers |
| log / env_logger | MIT OR Apache-2.0 | Logging |
| libc | MIT OR Apache-2.0 | System calls |
| futures | MIT OR Apache-2.0 | Async utilities |

### JavaScript (Frontend)

| Package | License | Purpose |
|---------|---------|---------|
| react / react-dom | MIT | UI framework |
| @tauri-apps/api | MIT | Tauri IPC bridge |
| i18next / react-i18next | MIT | Internationalization |
| react-markdown | MIT | Markdown rendering |
| tailwindcss | MIT | CSS framework |
| vite | MIT | Build tool |
| typescript | Apache-2.0 | Type system |

---

## MPL-2.0 Dependencies (Weak Copyleft)

The following crates are licensed under MPL-2.0. This is a file-level copyleft license: if you modify these specific source files, the modifications must be made available under MPL-2.0. Fresh Mayhem does not modify any of these files — they are compiled unmodified as transitive dependencies of Tauri's WebKitGTK integration.

| Crate | Purpose |
|-------|---------|
| cssparser | CSS parsing (Tauri internal) |
| cssparser-macros | CSS parser macros (Tauri internal) |
| dtoa-short | Float-to-string conversion (Tauri internal) |
| selectors | CSS selector matching (Tauri internal) |
| option-ext | Option type extensions (dirs crate) |

MPL-2.0 is explicitly compatible with proprietary software. See: https://www.mozilla.org/en-US/MPL/2.0/FAQ/

---

## External Tools (Not Bundled)

The following tools are called as separate processes via the system PATH. They are **not linked, bundled, or compiled into** Fresh Mayhem. Users install these independently.

| Tool | License | Source |
|------|---------|--------|
| hackrf_info | GPLv2 | Great Scott Gadgets |
| hackrf_transfer | GPLv2 | Great Scott Gadgets |
| hackrf_sweep | GPLv2 | Great Scott Gadgets |
| hackrf_debug | GPLv2 | Great Scott Gadgets |
| hackrf_clock | GPLv2 | Great Scott Gadgets |
| hackrf_biast | GPLv2 | Great Scott Gadgets |
| hackrf_operacake | GPLv2 | Great Scott Gadgets |

These tools are part of the [libhackrf](https://github.com/greatscottgadgets/hackrf) project by Great Scott Gadgets, licensed under GPLv2. Fresh Mayhem communicates with them via standard process execution (stdin/stdout), which does not create a derivative work under GPL terms.

---

*This file was generated on 2026-03-26. Run `cargo tree --format "{p} {l}"` for the current full dependency tree.*
