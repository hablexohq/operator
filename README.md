# Hablexo Operator

**Real-time translation for live services and events.** Hablexo listens to the speaker,
transcribes and translates on the fly, and delivers live captions to each attendee's phone in
their chosen language — they just scan a QR code. It can also translate projected song lyrics and
show them lower-third style.

This repository is the **download home** for the Hablexo operator app. Grab a build from the
[**Releases**](../../releases/latest) page.

## Download

| Platform | File | |
|---|---|---|
| **Windows** (installer) | `Hablexo-Setup.exe` | Recommended. One-click install to `C:\Program Files\Hablexo`, with Start-menu shortcuts. |
| **Windows** (portable) | `hablexo-operator-windows.zip` | Unzip anywhere and run `hablexo-operator.exe` inside the folder. |
| **macOS** | `hablexo-operator-macos.zip` | Unzip to get `hablexo-operator.app`, then launch. |
| **Linux** (x86-64) | `hablexo-operator-linux-x86_64.tar.gz` | Extract and run `./hablexo-operator/hablexo-operator`. |

### Install on Windows
1. Download and run **`Hablexo-Setup.exe`**.
2. It isn't code-signed yet, so Windows SmartScreen may warn — click **More info → Run anyway**.
3. Open **Hablexo Settings** from the Start menu to configure it, then launch **Hablexo**.

### Install on macOS
1. Download and unzip **`hablexo-operator-macos.zip`**.
2. macOS quarantines downloaded apps. Clear it once from Terminal:
   ```bash
   xattr -dr com.apple.quarantine hablexo-operator.app
   ```
3. Open the app and allow microphone access when prompted.

### Install on Linux (x86-64)
1. Download and extract **`hablexo-operator-linux-x86_64.tar.gz`**:
   ```bash
   tar -xzf hablexo-operator-linux-x86_64.tar.gz
   ```
2. Launch the app:
   ```bash
   ./hablexo-operator/hablexo-operator
   ```

## What you'll need

Hablexo runs on your own machine and connects **outbound only** to the Hablexo server — no inbound
ports, no port-forwarding. On first run, open the in-app **Settings** to sign in and configure your
event. Any provider credentials stay on your computer — they are never shared with attendees or
embedded in the web pages.

## How it works

1. Launch the app; it opens a local control panel in your browser.
2. Press **Start** and pick your audio source.
3. Share the on-screen **QR code** with attendees — scanning it opens the captions page for your
   event, in their chosen language.

---

© Hablexo. Releases are published automatically from our build pipeline.
