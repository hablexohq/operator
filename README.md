# EveryVox Live

**Real-time translation for live services and events.** EveryVox Live listens to the speaker,
transcribes and translates on the fly, and delivers live captions to each attendee's phone in
their chosen language — they just scan a QR code. It can also translate projected song lyrics and
show them lower-third style.

This repository is the **download home** for the EveryVox Live operator app. Grab a build from the
[**Releases**](../../releases/latest) page.

## Download

| Platform | File | |
|---|---|---|
| **Windows** (installer) | `EveryVox-Live-Setup.exe` | Recommended. One-click install to `C:\Program Files\EveryVox Live`, with Start-menu shortcuts. |
| **Windows** (portable) | `church-translate-operator-windows.zip` | Unzip anywhere and run the `.exe` inside the folder. |
| **macOS** | `church-translate-operator-macos.zip` | Unzip to get the app, then launch. |

### Install on Windows
1. Download and run **`EveryVox-Live-Setup.exe`**.
2. It isn't code-signed yet, so Windows SmartScreen may warn — click **More info → Run anyway**.
3. Open **EveryVox Live Settings** from the Start menu to enter your keys and token, then launch
   **EveryVox Live**.

### Install on macOS
1. Download and unzip **`church-translate-operator-macos.zip`**.
2. macOS quarantines downloaded apps. Clear it once from Terminal:
   ```bash
   xattr -dr com.apple.quarantine church-translate-operator.app
   ```
3. Open the app and allow microphone access when prompted.

## What you'll need

EveryVox Live runs on your own machine and connects out to your translation server. On first run,
open the settings and provide:

- your **Anthropic API key** (translation),
- your **Google Speech-to-Text** credentials (transcription),
- your **publish token** for the EveryVox Live server.

These stay on your computer — they are never shared with attendees or embedded in the web pages.

## How it works

1. Launch the app; it opens a local control panel in your browser.
2. Press **Start** and pick your audio source.
3. Share the on-screen **QR code** with attendees — scanning it opens the captions page for your
   event, in their chosen language.

---

© EveryVox Live. Releases are published automatically from our build pipeline.
