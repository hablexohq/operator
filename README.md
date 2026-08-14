# Hablexo Operator

**Real-time translation for live events.** Hablexo listens to the speaker,
transcribes and translates on the fly, and delivers live captions and speech to each attendee's phone in
their chosen language — they just scan a QR code. It can also translate projected NDI lyrics and
show them lower-third style.

This repository is the **download home** for the Hablexo operator app. Grab a build from the
[**Releases**](../../releases/latest) page.

## Download

| Platform | File | |
|---|---|---|
| **Windows** (installer) | `Hablexo-Setup.exe` | Recommended. One-click install to `C:\Program Files\Hablexo`, with Start-menu shortcuts. |
| **Windows** (portable) | `hablexo-operator-windows.zip` | Unzip anywhere and run `hablexo-operator.exe` inside the folder. |
| **macOS** | `hablexo-operator-macos.dmg` | Open the disk image and drag **Hablexo Operator** into Applications. |
| **Linux** (x86-64) | `hablexo-operator-linux-x86_64.tar.gz` | Extract and run `./hablexo-operator/hablexo-operator`. |

### Install on Windows
1. Download and run **`Hablexo-Setup.exe`**.
2. It isn't code-signed yet, so Windows SmartScreen may warn — click **More info → Run anyway**.
3. Open **Hablexo Settings** from the Start menu to configure it, then launch **Hablexo**.

### Install on macOS
1. Download and open **`hablexo-operator-macos.dmg`**.
2. Drag **Hablexo Operator** onto the **Applications** shortcut in the same window.
3. Launch it from Applications. The first time, macOS asks you to confirm an app downloaded from
   the internet — click **Open**.
4. Allow microphone access when prompted.

The macOS app is signed with our Apple Developer ID and notarized by Apple, so it opens without a
Gatekeeper warning. You do **not** need to clear the quarantine attribute by hand.

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
