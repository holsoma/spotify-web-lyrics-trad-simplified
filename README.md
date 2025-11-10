# Spotify Lyrics: Traditional ⇄ Simplified Chinese

🎶 A lightweight Tampermonkey userscript that automatically converts Spotify's fullscreen lyrics between **Traditional** and **Simplified Chinese**, with a small in-panel toggle (`繁 / 简`) and `Alt + L` keyboard shortcut.

---

### 🎥 Demo
![Image](https://github.com/user-attachments/assets/ce21a5ae-5324-4365-948f-4f4c516a4a86)

---

### ✨ Features
- ✅ Works **only inside Spotify Web’s fullscreen lyrics panel** (`data-testid="fullscreen-lyric"`)
- ✅ Automatically converts Traditional → Simplified Chinese on load
- ✅ Toggle between both forms with a small translucent **“繁 / 简”** button
- ✅ Keyboard shortcut: **Alt + L** (Option + L on macOS)
- ✅ Stores each line’s original Traditional text for perfect reversibility
- ✅ Uses the reliable **OpenCC** engine for accurate conversion
- ✅ Tested and confirmed working on **Firefox + Tampermonkey v5.x**

---

### 🖥️ Installation & Usage

#### 1️⃣ Install a Userscript Manager
You’ll need a browser extension to run the script:

- 🦊 **[Tampermonkey for Firefox](https://addons.mozilla.org/firefox/addon/tampermonkey/)** *(tested & verified working)*
- 🧩 **[Tampermonkey for Chrome / Edge](https://tampermonkey.net/?ext=dhdg&browser=chrome)**

> ⚙️ This script was developed and tested primarily using **Firefox (Tampermonkey v5.x)**.

---

#### 2️⃣ Install the Script
Click below to install directly from GreasyFork:

👉 **[Install from GreasyFork](https://greasyfork.org/en/scripts/555411-spotify-lyrics-trad-simplified)**

Tampermonkey will automatically handle installation and future updates.  
*(Advanced users may also install directly from the GitHub Raw link.)*

---

#### 3️⃣ Open Spotify Web Player
1. Visit **[https://open.spotify.com](https://open.spotify.com)**  
2. Play any song and open **Fullscreen Lyrics** (click the 🎤 icon).  
3. You’ll see the **“繁 / 简”** toggle appear in the bottom-right corner of the lyrics panel.

---

#### 4️⃣ Usage Controls
| Action | Description |
|:--|:--|
| **繁 / 简 button** | Switch between Traditional and Simplified Chinese |
| **Alt + L** | Keyboard toggle (Option + L on macOS) |
| **Default mode** | Simplified Chinese (converted using [OpenCC](https://github.com/BYVoid/OpenCC)) |

---

### 🧩 Technical Details
- Written in plain JavaScript (no frameworks)
- Uses [`opencc-js`](https://www.npmjs.com/package/opencc-js) via jsDelivr CDN
- Employs MutationObservers + periodic sweeps to handle Spotify’s dynamic lyric updates
- Works with Firefox, Chrome, and Edge

---

### 🧠 Developer Notes
If you’d like to modify or self-host:
1. Fork this repo.
2. Edit [`spotify-web-lyrics-trad-simplified.user.js`](./spotify-web-lyrics-trad-simplified.user.js).
3. Commit and push your changes.
4. The Raw URL acts as a Tampermonkey install/update link.

To test locally:
```bash
https://raw.githubusercontent.com/holsoma/spotify-web-lyrics-trad-simplified/main/spotify-web-lyrics-trad-simplified.user.js
