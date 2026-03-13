# Installing SONU

## Download

Get the latest release for your platform from [GitHub Releases](https://github.com/ai-dev-2024/sonu/releases).

| Platform | Format | File |
|----------|--------|------|
| **Windows x64** | Installer | `SONU_x.x.x_x64-setup.exe` |
| **Windows x64** | MSI | `SONU_x.x.x_x64_en-US.msi` |
| **Windows ARM64** | Installer | `SONU_x.x.x_arm64-setup.exe` |
| **macOS Apple Silicon** | DMG | `SONU_x.x.x_aarch64.dmg` |
| **macOS Intel** | DMG | `SONU_x.x.x_x64.dmg` |
| **Linux (Ubuntu 24.04+)** | AppImage | `SONU_x.x.x_amd64.AppImage` |
| **Linux (Ubuntu 24.04+)** | RPM | `SONU-x.x.x-1.x86_64.rpm` |
| **Linux (Ubuntu 22.04)** | Deb | `SONU_x.x.x_amd64.deb` |

## Platform Notes

### Windows
Run the `.exe` installer. If SmartScreen warns you, click **"More info"** → **"Run anyway"**.

### macOS
Open the `.dmg`, drag SONU to Applications. On first launch: right-click → **"Open"** → **"Open"**.

### Linux
```bash
chmod +x sonu_*.AppImage
./sonu_*.AppImage
```

Or install the `.deb`:
```bash
sudo dpkg -i sonu_*.deb
```

## Why Unsigned?

SONU is free and open-source. Code signing certificates cost $300+/year. Your security comes from transparent code at [github.com/ai-dev-2024/sonu](https://github.com/ai-dev-2024/sonu).

## Building from Source

**Prerequisites**: [Bun](https://bun.sh), [Rust toolchain](https://rustup.rs), platform-specific Tauri v2 dependencies.

```bash
git clone https://github.com/ai-dev-2024/sonu.git
cd sonu/apps/tauri-v2
bun install
bun run tauri dev    # Development
bun run tauri build  # Production build
```

See [Tauri v2 Prerequisites](https://v2.tauri.app/start/prerequisites/) for system-level dependencies.

