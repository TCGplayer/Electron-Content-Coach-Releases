# 📦 Content Coach Installation Guide

## 🚀 Quick Installation (Recommended)

```bash
curl -fsSL https://raw.githubusercontent.com/TCGplayer/Electron-Content-Coach-Releases/main/install.sh | bash
```

This script will:
- ✅ Download the latest version automatically
- ✅ Install to your Applications folder
- ✅ Remove quarantine attributes for seamless first launch
- ✅ Offer to launch the app immediately

> **Note:** GitHub downloads may fail if you are on the eBay VPN. Disconnect VPN before running the installer, then reconnect after.

## 📥 Manual Installation

1. Go to the [Releases page](https://github.com/TCGplayer/Electron-Content-Coach-Releases/releases)
2. Download the latest `Content-Coach-X.X.X-arm64.dmg`
3. Open the DMG and drag **Content Coach** to `/Applications`
4. Right-click the app and select **Open** (required on first launch due to macOS Gatekeeper)

## 🔄 Updates

Content Coach checks for new versions on launch and shows a notification banner when an update is available. To update, re-run the installer or download the new DMG manually.

## 🛠️ Requirements

- **macOS 12.0** or later (Apple Silicon recommended)
- **eBay VPN** connected while using the app (required for AI processing)
- No other setup needed — Python and all dependencies are bundled

## 🚨 Troubleshooting

### "App can't be opened" on first launch
macOS Gatekeeper blocks unsigned apps by default:
1. Right-click **Content Coach** in Applications
2. Select **Open**
3. Click **Open** in the security dialog

### Updates not appearing
The app checks for updates on launch. If no banner appears, you are on the latest version. You can also check the [Releases page](https://github.com/TCGplayer/Electron-Content-Coach-Releases/releases) directly.

### AI processing not working
- Ensure the eBay VPN is connected
- The VPN warning banner in the app will indicate connectivity status

## 🆘 Support

Contact the development team or open an issue in the [source repository](https://github.com/TCGplayer/Electron_Content_Coach).
