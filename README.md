<div align="center">
  <img alt="GUI Screenshot" src="https://github.com/dfleury2/boss-rc500-editor/raw/master/docs/images/screenshot.png" height="500" />
</div>
<br>


# Unofficial Boss RC-500 Editor – macOS Apple Silicon Build

This repository provides **unofficial macOS Apple Silicon (arm64)** builds of  
[dfleury2/boss-rc500-editor](https://github.com/dfleury2/boss-rc500-editor),  
an open-source configuration editor for the **Boss RC-500 Loop Station**.

> ⚠️ Disclaimer  
> This project is **not affiliated with BOSS / Roland** or the original author.  
> Use at your own risk and always back up your RC-500 before making changes.

The upstream project is MIT-licensed. See [LICENSE](LICENSE) for details.

---

## Download

1. Go to the **[Releases](../../releases)** page.
2. Download the latest file named:

   `BossRc500-Editor-0.0.10-macos-arm64.zip`

3. Unzip it. You should get:

   ```text
   BossRc500-Editor-0.0.10-macos-arm64/
     ├── BossRc500
     └── resources/
Running on macOS (Apple Silicon)
Open Terminal.

Change into the unzipped folder, for example:

bash
Copy code
cd /path/to/BossRc500-Editor-0.0.10-macos-arm64
Make the binary executable (one-time):

bash
Copy code
chmod +x BossRc500
Run the editor:

bash
Copy code
./BossRc500
The program expects to run from that folder so it can find ./resources for fonts and themes.

macOS security prompt
First run, macOS may block it as “unidentified developer”:

Right-click BossRc500 → Open → confirm,

Or allow it under System Settings → Privacy & Security.

Connecting to your RC-500
On the RC-500:
MENU → STORAGE → connect via USB to your Mac.

On macOS, a drive named “BOSS RC-500” appears.

In the editor: File → Open…

Open BOSS RC-500/ROLAND/DATA.

Edit memories as desired, then eject the “BOSS RC-500” drive in Finder and exit STORAGE mode on the pedal.

Upstream project
All application code & credit belong to:

Project: dfleury2/boss-rc500-editor

Docs: https://dfleury2.github.io/boss-rc500-editor/

Please report application bugs or feature requests to the upstream project.
This repo only distributes prebuilt macOS arm64 binaries.

yaml
Copy code

Note: everything here is generic – no machine paths, no usernames.

---

## 5. (Optional) Add `RELEASE_NOTES.md`

This is nice but not mandatory. From your small repo:

```bash
nano RELEASE_NOTES.md
Paste something like:

markdown
Copy code
# Release Notes – Unofficial Boss RC-500 Editor macOS arm64

## v0.0.10-arm64-1

- Built from upstream dfleury2/boss-rc500-editor tag `v0.0.10`.
- Target: **macOS Apple Silicon (arm64)**.
- Toolchain:
  - Apple Clang (Xcode command line tools)
  - CMake
  - Conan 1.x for dependencies
- Build type: `Release` (binary stripped of debug symbols).

### Notes

- No functional changes to the application logic compared to upstream.
- Minor macOS build adjustments only (Qt configuration, etc.).
- The application is still considered alpha by the original author.
