# EOS Webcam Utility – Free Version Archive Links

Canon discontinued the free **EOS Webcam Utility** on **August 20, 2025** and replaced it with the subscription-based **EOS Webcam Utility Pro**. The free installers were removed from Canon's download servers and regional websites.

This repository collects **links to archived copies of Canon's original installers** on the Internet Archive's Wayback Machine, with SHA-256 checksums wherever one has been verified, so you can confirm you're getting the untouched original.

**Quick start (Windows):** download the **1.3.16** zip below → check its SHA-256 → check `Setup.exe` is signed by Canon → install → restart.

> **This repository does not host any Canon software.** Every link points to an archived copy of a file Canon itself distributed for free from `downloads.canon.com`. EOS Webcam Utility is © Canon Inc.

---

## Downloads

**Most people want the first row for their platform.** Older versions are listed in case a newer one doesn't work with your camera or OS.

### Windows

| Version | Download | All snapshots | Archived between | SHA-256 |
|---|---|---|---|---|
| **1.3.16** (final free release) | [EOSWebcamUtility-WIN1.3.16.zip](https://web.archive.org/web/20250820111819/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.3.16.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.3.16.zip) | Apr 2024 – Aug 2025 | `653F776F2E3710A9C1358B973D20FA0C49C1565AF45CF8E3629D20A1D4F9B0BB` |
| 1.2 | [EOSWebcamUtility-WIN1.2.zip](https://web.archive.org/web/20230811091402/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.2.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.2.zip) | Oct 2022 – Aug 2023 | _unverified_ |
| 1.1 | [EOSWebcamUtility-WIN1.1.zip](https://web.archive.org/web/20230721055317/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.1.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.1.zip) | Jul 2021 – Sep 2025 | _unverified_ |
| 1.0 | [EOSWebcamUtility-WIN1.0.zip](https://web.archive.org/web/20230420192145/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.0.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-WIN1.0.zip) | Sep 2020 – Aug 2025 | _unverified_ |
| 0.9.0 Beta | [EOSWebcamUtilityBeta-WIN0.9.0.zip](https://web.archive.org/web/20241106180920/http://downloads.canon.com/webcam/EOSWebcamUtilityBeta-WIN0.9.0.zip) | [calendar](https://web.archive.org/web/*/http://downloads.canon.com/webcam/EOSWebcamUtilityBeta-WIN0.9.0.zip) | Jul 2020 – Nov 2024 | _unverified_ |

### macOS

| Version | Download | All snapshots | Archived between | SHA-256 |
|---|---|---|---|---|
| **1.3.16** (final free release) | [EOSWebcamUtility-MAC1.3.16.pkg.zip](https://web.archive.org/web/20250817190943/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.3.16.pkg.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.3.16.pkg.zip) | Aug 2025 | _unverified_ |
| 1.1 | [EOSWebcamUtility-MAC1.1.pkg.zip](https://web.archive.org/web/20231202032117/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.1.pkg.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.1.pkg.zip) | Jul 2023 – Dec 2023 | _unverified_ |
| 1.0 | [EOSWebcamUtility-MAC1.0.pkg.zip](https://web.archive.org/web/20220411062425/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.0.pkg.zip) | [calendar](https://web.archive.org/web/*/https://downloads.canon.com/webcam/EOSWebcamUtility-MAC1.0.pkg.zip) | Dec 2020 – Apr 2022 | _unverified_ |
| 0.9.0 Beta | [EOSWebcamUtilityBeta-MAC0.9.0.pkg.zip](https://web.archive.org/web/20221205165114/http://downloads.canon.com/webcam/EOSWebcamUtilityBeta-MAC0.9.0.pkg.zip) | — (single snapshot) | Dec 2022 | _unverified_ |

**Notes**
- A hash marked _unverified_ means nobody has yet downloaded that file, confirmed its Canon signature and submitted the hash. If you do, please open an issue or PR.
- The Windows 1.0 and 1.1 files were captured with **more than one distinct content**, and their later snapshots (after August 2025) are likely Canon's error page rather than the installer. The links above point to 2023 snapshots taken while the files were still live. If you pick another date from the calendar, check the signature on whatever you get.
- **If a link fails**, open its calendar link and try another snapshot date. To browse everything Canon hosted in that folder, use [this index](https://web.archive.org/web/*/downloads.canon.com/webcam/*).
- The same folder also contains archived **EOS Webcam Utility Pro** installers (2.x). Pro is a separate subscription product and is out of scope for this page.

---

## Verify Before Installing

Always verify the file, especially if you got it from somewhere other than the links above.

**1. Check the SHA-256 hash**

Windows (PowerShell):
```powershell
Get-FileHash .\EOSWebcamUtility-WIN1.3.16.zip -Algorithm SHA256
```

macOS / Linux:
```bash
shasum -a 256 EOSWebcamUtility-MAC1.3.16.pkg.zip
```

Where the table lists a hash, the output must match it. The comparison is not case-sensitive: PowerShell prints uppercase, `shasum` prints lowercase. A file marked _unverified_ has no reference hash yet, so rely on the signature check below.

**2. Check Canon's digital signature (Windows)**

Extract the zip, right-click `Setup.exe` → **Properties** → **Digital Signatures**. The signer should be **Canon U.S.A., Inc.** (sha256). Select it and click **Details**: Windows should report *"This digital signature is OK."* If it's unsigned, signed by anyone else, or the signature isn't OK, don't run it.

**2b. Check Canon's signature (macOS)**

Unzip the download, then run:
```bash
pkgutil --check-signature /path/to/EOSWebcamUtility.pkg
```
It should report `Status: signed by a developer certificate issued by Apple` with a Canon developer ID in the certificate chain. If it's unsigned or signed by someone else, don't install it.

---

## Installation (Windows)

1. Close **EOS Utility** if it's running, and stop it from launching when a camera is connected.
2. Run the installer.
3. **Restart your PC.** The camera often isn't detected until you do.
4. Set the camera to **movie mode** (on most models) and connect it over USB.
5. In OBS, Discord, Zoom, Teams, etc., choose **EOS Webcam Utility** as the camera.

**Tips**
- Use a dummy battery / AC adapter. Live view drains batteries quickly.
- Turn off auto power-off in the camera menu.
- Use manual focus to stop the lens hunting during calls.
- USB output is the camera's live view stream (typically ~1024×576, depending on the model). For true 1080p, use the camera's HDMI output with a capture card.

---

## macOS Users (Apple Silicon)

[Obednal97/eos-webcam-utility](https://github.com/Obednal97/eos-webcam-utility) is a community fork that patches the free macOS v1.3.16 to output 1080p (upscaled) and handles camera connection retries automatically. Its installer obtains Canon's original package rather than redistributing it. It's a separate third-party project that this repo hasn't reviewed, so check it yourself before running it.

---

## Confirmed Working

Tested a camera? Open an issue or pull request to add it.

| Camera | OS | Version | Result | Notes |
|---|---|---|---|---|
| _none reported yet_ | | | | |

---

## Contributing

Contributions are welcome, especially:
- Archived links to versions missing above (e.g. Windows 1.3.x releases between 1.2 and 1.3.16, or a macOS 1.2)
- Verified SHA-256 hashes, along with confirmation that the Canon signature checks out
- Results from your camera model

Please **don't** submit the installer files themselves. Links only.

---

## Disclaimer

This project is not affiliated with or endorsed by Canon Inc. Canon and EOS are trademarks of Canon Inc. It exists only to help owners of Canon cameras find the free software Canon previously provided for them. The software remains subject to Canon's original license terms. Use at your own risk.

If you represent Canon or the Internet Archive and want a link removed, please open an issue.
