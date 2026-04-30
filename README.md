# Now Utils — Productivity Tools for ServiceNow

A browser extension that enhances the ServiceNow experience with a suite of productivity tools, available directly from the toolbar or triggered inline while working on any ServiceNow instance.

---

## Features

### Slash Commands Menu
Type `/` in any ServiceNow field to open the command overlay. Built-in commands cover common navigation shortcuts, and you can define your own custom commands.

- **Modern dark UI** with a navy/teal color scheme
- **Drag-and-drop** — reposition the overlay anywhere on screen by dragging the header
- **Dark / Light toggle** — switch themes without leaving the page
- **Ghost theme** — fully transparent overlay, black text only, blends into any page
- **Export commands** — download all commands (built-in + custom) as a JSON file
- **Import commands** — load a JSON file; only new commands are added, existing ones are never overwritten

### Popup (Extension Toolbar)
Click the extension icon to open the popup panel:

- **Settings tab** — configure slash command theme (Dark, Light, Ghost), toggle switches, and other preferences
- **Slash Commands tab** — view, add, edit, and delete custom commands; Export / Import buttons for portability
- **Update Sets tab** — manage and inspect ServiceNow update sets
- **Node Switching** — quickly switch between nodes on your instance
- **GlideRecord Generator** — generate GlideRecord code templates
- **Technical Names toggle** — show or hide technical field names on any form

### Code Editor (Monaco)
Embedded Monaco editor for editing scripts directly in the browser, with syntax highlighting and a diff viewer.

### ScriptSync Integration
Sync scripts with VS Code via [sn-scriptsync](https://github.com/salcad/sn-scriptsync) for a local development workflow.

### Code Search
Full-text search across scripts on your ServiceNow instance.

### InstanceTag
Draggable instance-tag button that shows which environment you are working in.

### View Data
Inspect record field data in a structured view (`/vd` command).

---

## Installation

1. Clone or download this repository.
2. Open Chrome and navigate to `chrome://extensions/`.
3. Enable **Developer mode** (top-right toggle).
4. Click **Load unpacked** and select the repository folder.

The Now Utils icon will appear in your Chrome toolbar.

---

## Custom Slash Commands

### Adding a command
1. Open the popup and go to the **Slash Commands** tab.
2. Fill in the **Command**, **URL**, **Hint**, and optional **Fields** / **Order**.
3. Click **Save**.

### Exporting commands
Click the **Export** button in the Slash Commands tab to download all commands (built-in and custom) as `slashcommands.json.txt`.

### Importing commands
Click **Import**, select a JSON file exported from another instance. Only commands that do not already exist will be added — no existing commands are overwritten.

---

## Themes

Select the slash commands overlay theme from **Settings → Slash Commands Theme**:

| Theme | Description |
|-------|-------------|
| Dark  | Navy background with teal accents (default) |
| Light | White background with green accents |
| Ghost | Fully transparent — text only, no background or border |

The overlay also has a per-session **☀ / 🌙 toggle** in its header to switch between dark and light without changing the saved setting.

---

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Cmd+1` / `Ctrl+1` | Activate / open extension |
| `Cmd+2` / `Ctrl+2` | Pop in / Pop out |
| `Cmd+3` / `Ctrl+3` | Toggle Technical Names |

Shortcuts can be customised at `chrome://extensions/shortcuts`.

---

## Contributing

Open an issue to discuss a new feature before starting development. Pull requests submitted without prior discussion may not be reviewed.

---

## Privacy

Now Utils does not collect, transmit, or store any personal data or browsing history. All settings are saved locally in your browser's storage. Required browser permissions are used solely to interact with ServiceNow pages on the active tab.
