# BrásCubas

> *Named after a famous literary character who wasted his entire life on distractions, BrásCubas is the ultimate blocker that stops you from meeting the same fate.*

Intentional YouTube feed building. Curate sources, organize by topic, generate a focused feed — and watch it in a distraction-free local Focus Player.

---

## Installation

BrásCubas has two parts:

| Part | What it does | How to install |
|---|---|---|
| **Chrome Extension** (`.crx`) | Feed Builder UI, topic management, feed generation | Install manually in Chrome |
| **Companion App** (`.pkg`) | Runs the local Focus Player server + connects it to Chrome | Run the macOS installer |

Both are available on the [Releases page](https://github.com/andrewrosemberg/BrasCubasLite/releases).

---

### Step 1 — Install the Chrome Extension

1. Download `BrasCubas-<version>.crx` from the [latest release](https://github.com/andrewrosemberg/BrasCubasLite/releases/latest).
2. Open `chrome://extensions` in Chrome.
3. Enable **Developer mode** (toggle in the top-right corner).
4. Drag and drop the `.crx` file onto the extensions page.
5. Click **Add extension** in the confirmation dialog.

> **Blocked by Chrome?** Chrome may warn about extensions installed outside the Web Store.
> If the extension is removed automatically, try the unpacked method instead:
> rename the `.crx` to `.zip`, extract it, then click **Load unpacked** and select the extracted folder.

---

### Step 2 — Install the Companion App (macOS)

The Companion App installs the local Focus Player server and registers it with Chrome so it starts automatically whenever you click **Open Focus Player**.

1. Download `BrasCubas-Companion-<version>.pkg` from the [latest release](https://github.com/andrewrosemberg/BrasCubasLite/releases/latest).
2. Double-click the `.pkg` file to run the installer.

> **macOS security warning?** Right-click the file → **Open** → click **Open** in the dialog.
> This is expected for software distributed outside the Mac App Store.

3. Follow the installer steps (no configuration needed — just click through).
4. After installation, **reload the BrásCubas extension** in `chrome://extensions`.
5. Open BrásCubas, build a feed, and click **Open Focus Player**.

The server starts automatically in the background — no terminal required.

---

### Updating

To update either part, download the new version from the [Releases page](https://github.com/andrewrosemberg/BrasCubasLite/releases) and repeat the relevant step above. The Companion App installer handles updates in-place.

---

## Usage

1. Open the BrásCubas popup from the Chrome toolbar.
2. Click **Feed Builder** to open the full app.
3. Add YouTube channels, playlists, or videos as sources.
4. Organize them by topic, set per-source limits, and click **Regenerate Feed**.
5. Click **Open Focus Player** to watch your feed distraction-free.

---

## Focus Player

The Focus Player is a local web app served by the Companion App. It provides:
- Distraction-free playback (no recommendations, no comments)
- Autoplay queue with shuffle
- Watch progress tracking synced back to BrásCubas
- Topic-grouped queue display

---

## Troubleshooting

Open the **⚙ Local Viewer** panel in the Feed Builder's left rail for:
- Connection testing
- Error log with copy-to-clipboard
- Direct link to this issues page

**Common issues:**

| Symptom | Fix |
|---|---|
| "Companion app is not installed" | Install the `.pkg` from the releases page, then reload the extension |
| "Could not reach local Focus Player" | Click **Test Connection** in the ⚙ panel — if it fails, try restarting Chrome |
| macOS blocked the installer | Right-click → Open → Open |
| Extension removed by Chrome | Rename `.crx` → `.zip`, extract, Load unpacked |

---

[Report an issue](https://github.com/andrewrosemberg/BrasCubasLite/issues)
