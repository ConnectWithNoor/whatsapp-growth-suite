<div align="center">

# WhatsApp Growth Suite

**Send personalized WhatsApp messages to hundreds of contacts — from your own number, on your own machine.**

[Download for Windows](https://github.com/ConnectWithNoor/whatsapp-growth-suite/releases/download/release/whatsapp-growth-suite-1.0.0-setup.exe) &nbsp;·&nbsp; [Download for Mac](#-download) - Coming Soon &nbsp;·&nbsp; [Download for Linux](#-download) - Coming Soon &nbsp;·&nbsp; [Quick Start](#-quick-start) &nbsp;·&nbsp; [Support](#-support)

---

</div>

## What is WhatsApp Growth Suite?

WhatsApp Growth Suite is a desktop app that lets you send bulk WhatsApp messages directly from your own WhatsApp account. No third-party API keys. No per-message fees. No cloud dependency. Your messages go out exactly as if you sent them yourself — just at scale.

Perfect for small businesses, marketers, coaches, and community managers who want to reach their audience on WhatsApp without the complexity or cost of enterprise solutions.

---

## Download

> **Always download from this page.** Never trust links from third parties.

Head to the **[Releases](../../releases/latest)** tab and grab the file for your platform:

| Platform | File | Notes |
|----------|------|-------|
| **Windows** | `whatsapp-growth-suite-x.x.x-setup.exe` | Windows 10 / 11 (64-bit) |
| **macOS** | `whatsapp-growth-suite-x.x.x.dmg` | macOS 12 Monterey or later |
| **Linux** | `whatsapp-growth-suite-x.x.x.AppImage` | Works on most distros |
| **Linux (Debian/Ubuntu)** | `whatsapp-growth-suite-x.x.x.deb` | Ubuntu 20.04+ / Debian |

---

## Features at a Glance

| | |
|--|--|
| **QR-based WhatsApp login** | Connect your number in seconds — no API keys, no credentials stored |
| **Contact audiences** | Import contacts from CSV/Excel or add them manually |
| **WhatsApp group targeting** | Sync your existing groups and use them as campaign recipients |
| **Group Forwarding** | Bypass 5 groups forward only limitation |
| **Personalized messages** | Use `{{name}}`, `{{phone}}`, or any custom field from your contact list |
| **Media attachments** | Send images, videos, audio, PDFs, and documents alongside your message |
| **Smart sending engine** | Configurable delays with ±20% randomization so sends look natural |
| **Auto-rest intervals** | Pause automatically after every N messages to stay under the radar |
| **Pause / Resume / Stop** | Full control over every running campaign at any time |
| **Crash-safe resuming** | If you close the app mid-campaign, reopen and resume — no duplicates |
| **Dashboard stats** | Campaigns, contacts, audiences, sent and failed counts at a glance |

---

## Quick Start

### Step 1 — Install the app

**Windows:** Run the `.exe` installer. A desktop shortcut is created automatically.

**macOS:** Open the `.dmg` file, drag the app to your **Applications** folder, and open it from there.

> On macOS you may see a security warning on first open because the app is not notarized by Apple. To bypass it: **right-click the app → Open → Open anyway.**

**Linux (AppImage):**
```bash
chmod +x whatsapp-growth-suite-*.AppImage
./whatsapp-growth-suite-*.AppImage
```

**Linux (Debian/Ubuntu):**
```bash
sudo dpkg -i whatsapp-growth-suite-*.deb
```

---

### Step 2 — Connect your WhatsApp

Go to **Connection** in the sidebar and scan the QR code with your phone:

1. Open **WhatsApp** on your phone
2. Tap **Settings → Linked Devices → Link a Device**
3. Point your camera at the QR code shown in the app

Once connected, your phone number and profile name appear in the app. The session is saved locally — you only need to scan once.

---

### Step 3 — Create an audience

Go to **Audiences** → **New Audience** and choose how to add your recipients:

**From a CSV or Excel file:**
- Your file needs at least a `name` column and a `phone` column
- Any additional columns (e.g. `city`, `plan`, `discount`) can be used as message variables
- Phone numbers can be in any common format — the app handles the formatting

**From your WhatsApp groups:**
- Switch to the **Groups** tab
- Your synced groups appear here — add them to an audience with one click

---

### Step 4 — Create and run a campaign

Go to **Campaigns** → **New Campaign** and fill in the three tabs:

| Tab | What to do |
|-----|-----------|
| **Audience** | Pick which audience receives the campaign |
| **Message** | Write your message, insert personalization variables, and optionally attach a file |
| **Settings** | Set delay between messages, auto-rest frequency, and rest duration |

Click **Create Campaign**, then click **Start** on the campaign detail page. The app sends messages one by one and shows live progress.

You can **Pause** at any time, come back later, and **Resume** — contacts who already received the message are never messaged again.

---

## Personalizing Your Messages

Variables are placeholders in your message that get replaced with each contact's data before sending.

| Variable | Replaced with |
|----------|--------------|
| `{{name}}` | The contact's name |
| `{{phone}}` | The contact's phone number |
| `{{column_name}}` | Any extra column from your imported CSV |

**Example:**
```
Hi {{name}}! We have a special offer for customers in {{city}} this week.
Reply YES to claim your {{discount}}% discount 🎉
```

Each recipient receives a message with their own values filled in. If a contact is missing a value for a variable, that placeholder is simply left blank.

> Variables work for contact-list audiences. For WhatsApp group audiences the same message is sent to all groups.

---

## Recommended Settings

These defaults work well for most accounts:

| Setting | Recommended value | Why |
|---------|------------------|-----|
| Delay between messages | **5 – 10 seconds** | Looks natural, reduces flag risk |
| Auto-rest after | **50 messages** | Mimics human break patterns |
| Rest duration | **5 – 10 minutes** | Enough of a gap to avoid detection |

The app applies a **±20% random variation** to your delay automatically — so if you set 5 seconds, each message waits somewhere between 4 and 6 seconds. This makes the sending pattern look human.

---

## System Requirements

| | Minimum |
|--|---------|
| **Windows** | Windows 10, 64-bit |
| **macOS** | macOS 12 Monterey |
| **Linux** | Ubuntu 20.04 or equivalent |
| **RAM** | 512 MB |
| **Storage** | 300 MB free |
| **Internet** | Required (WhatsApp connection) |

---

## FAQ

**Does this use the official WhatsApp Business API?**
No. It uses WhatsApp Backdoor APIs, Messages come directly from your personal or business number and appear as normal WhatsApp messages.


**Is Is Whatsapp Growth Suite safe to use?**
Whatsapp Growth Suite is designed to comply with relevant regulations and industry standards, prioritizing user security and privacy.
You can trust us for a secure and reliable experience.

**Can I run this on two computers?**
One license is tied to one machine. To transfer to a new computer, contact support and we can help.

**The QR code expired before I could scan it.**
A new QR code is generated automatically. Wait a moment for it to refresh, then try scanning again.

**A campaign is stuck on "Running" after I restarted.**
On startup the app automatically moves stuck campaigns to "Paused". Open the campaign and click **Resume**.

**Can I send to multiple audiences at once?**
Each campaign targets one audience. To reach multiple lists, create separate campaigns.

**What file types can I attach?**
Images (JPG, PNG, GIF, WebP), videos (MP4, MOV, AVI, WebM), audio (MP3, WAV, OGG, M4A), and documents (PDF, DOCX, DOC).

---

## Support

Having trouble or have a question?

- **WhatsApp:** Chat with us directly via the link on [whatsappgrowthsuite.com](https://whatsappgrowthsuite.com)
- **Website:** [whatsappgrowthsuite.com](https://whatsappgrowthsuite.com)

When reaching out, please include:
- Your operating system (Windows 11, macOS 14, Ubuntu 22.04, etc.)
- The app version number
- A brief description of what happened and what you were doing

---

## Changelog

See the [Releases](../../releases) tab for the full version history and release notes.

---

<div align="center">

Made with care by **Revera Innovations**

[reverainnov.com](https://reverainnov.com)

</div>
