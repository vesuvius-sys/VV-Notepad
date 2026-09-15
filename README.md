# VVNotepad

**A password-locked notepad for Windows. Everything stays on your PC.**

[![Platform](https://img.shields.io/badge/platform-x64%20%7C%20ARM64-blue?style=flat-square)](#requirements) [![License](https://img.shields.io/badge/license-closed--source%2C%20free-lightgrey?style=flat-square)](#license) [![Network](https://img.shields.io/badge/network-none-brightgreen?style=flat-square)](#privacy--data-handling)

VVNotepad encrypts what you type before it ever touches disk. No accounts, no cloud, no background sync — just notes, locked with a password only you know.

VVNotepad is made by **Vesuvius Systems**. If you want more control over your privacy on Windows, check out our other tool, [TWK3R](https://github.com/vesuvius-sys/TWK3R).

[About](#about) · [Features](#features) · [How to Use](#how-to-use) · [Privacy & Data Handling](#privacy--data-handling) · [FAQ](#faq) · [License](#license)

---

## About

Most "secure" notepads either don't really encrypt anything, or quietly sync your notes somewhere in the background. VVNotepad does neither — it's a plain desktop notepad that locks your notes with real encryption and has no code path that can send anything anywhere.

Your password becomes the encryption key using **AES-256-GCM**, the same standard used to protect classified government data. The password itself is never stored — only a random "salt" value needed to rebuild the key next time, which is useless without the password. There's no reset option by design: if the app could recover your password, the lock wouldn't mean much.

---

## Features

|                          |                                                                                       |
| ------------------------ | ------------------------------------------------------------------------------------- |
| 🔒 **Password lock**      | AES-256-GCM encryption, key derived from your password — no recovery path, on purpose |
| 📑 **Multiple notes**     | Drag to reorder, rename, delete — each one encrypted separately                       |
| 🖼 **Embedded images**    | Including animated GIFs, placed anywhere on the page, encrypted like your text        |
| 🎨 **Per-selection color/size** | Highlight any text and change just its color or size — saved permanently        |
| ↩ **Real undo/redo**     | A whole sentence undoes at once, like Notepad or Word — plus a ~25s "big undo"        |
| 🌗 **Eight themes**       | Switch instantly, no restart needed                                                   |

---

## How to Use

1. Open the app and set a password. Type it again to confirm.
2. Start typing — your note saves itself, no need to hit save.
3. Click **[ + NEW NOTE ]** to add another note.
4. Right-click in a note to add a picture, or to change the color/size of selected text.
5. Next time you open the app, enter the same password to get back in.

---

## Privacy & Data Handling

**No network calls, ever.** No telemetry, no update pinging, no analytics, nothing sent anywhere. Every note is written only to your own machine.

Beyond your own password (which is never itself saved), VVNotepad has no servers, no accounts, and nothing on our end to collect anything. 🚫

---

## FAQ

<details>
<summary><b>What happens if I forget my password?</b></summary>
<br>
Your notes can't be recovered. This is intentional — a recoverable password would mean the encryption isn't really protecting anything.
</details>

<details>
<summary><b>Does closing the app save my notes?</b></summary>
<br>
Yes — notes save automatically as you type, and again on close.
</details>

<details>
<summary><b>Can I move my notes to another PC?</b></summary>
<br>
Yes, copy the encrypted notes folder over and unlock it with the same password on the other machine.
</details>

<details>
<summary><b>Is the source code public?</b></summary>
<br>
No — VVNotepad is closed-source and free to use, with no EULA to sign.
</details>

---

## Requirements

Windows 10 or 11 (x64 or ARM64), with the free **.NET 8** runtime — the app will tell you if it's missing.

## License

Closed-source, free to use. No warranty, no support commitment — a personal project, maintained as time allows.
