# Unofficial Boss RC-500 Editor – macOS Apple Silicon Build

This repository provides **unofficial macOS Apple Silicon (arm64)** builds of
[dfleury2/boss-rc500-editor](https://github.com/dfleury2/boss-rc500-editor),
an open-source configuration editor for the **Boss RC-500 Loop Station**.

> ⚠️ **Disclaimer**  
> This project is not affiliated with BOSS / Roland or the original author.  
> Use at your own risk and always back up your RC-500 before making changes.

The upstream project is MIT-licensed. See [LICENSE](LICENSE) for details.

---

## Download

1. Go to the [Releases](../../releases) page.
2. Download the latest file named, for example:

   ```text
   BossRc500-Editor-0.0.10-macos-arm64.zip
   ```

3. Unzip it. You should get:

   ```text
   BossRc500-Editor-0.0.10-macos-arm64/
   ├── BossRc500
   └── resources/
   ```

---

## Running on macOS (Apple Silicon)

1. Open **Terminal**.
2. Change into the unzipped folder, for example:

   ```bash
   cd /path/to/BossRc500-Editor-0.0.10-macos-arm64
   ```

3. Make the binary executable (one-time):

   ```bash
   chmod +x BossRc500
   ```

4. Run the editor:

   ```bash
   ./BossRc500
   ```

The program expects to run from that folder so it can find `./resources` for fonts and themes.

### macOS security prompt

On first run, macOS may block it as “unidentified developer”:

- Right-click `BossRc500` → **Open** → confirm, or  
- Allow it under **System Settings → Privacy & Security**.

---

## Connecting to your RC-500

1. On the RC-500:  
   `MENU → STORAGE`, then connect via USB to your Mac.
2. On macOS, a drive named **“BOSS RC-500”** appears.
3. In the editor: **File → Open…** and open:

   ```text
   BOSS RC-500/ROLAND/DATA
   ```

4. Edit memories as desired.
5. In Finder, **eject** the “BOSS RC-500” drive and then exit STORAGE mode on the pedal.

---

## Upstream project

All application code & credit belong to:

- **Project:** [dfleury2/boss-rc500-editor](https://github.com/dfleury2/boss-rc500-editor)  
- **Docs:** https://dfleury2.github.io/boss-rc500-editor/

Please report application bugs or feature requests to the upstream project.  
This repo only distributes prebuilt **macOS arm64** binaries.
