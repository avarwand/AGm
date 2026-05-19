# AGm | Avarwand Git Manager

A professional **graphical Git repository manager**, designed to manage
multiple local Git repositories simultaneously, with batch operations,
live status monitoring, an interactive CLI, submodule management, and a
fully configurable dark-themed interface.

---

## Main Features

### Profile Management
- 📁 **Multiple Repository Profiles**: Add, edit, and remove any number of
  local Git repository paths as named profiles.
- 📂 **Import Folders**: Select multiple folders at once, AGm automatically
  detects valid Git repositories and imports them in a single step.
  Duplicate paths are detected and skipped automatically.
- 🟢🔴 **Live Status Colours**: Each profile is automatically colour-coded
  after every operation, green for clean repositories (nothing to commit),
  dark red for repositories with untracked or modified files.
- 🔍 **Search & Filter**: Type to filter profiles by name. Use the
  **✅ Synced** and **🔴 Untracked** checkboxes to instantly show only
  clean or dirty repositories.
- 📊 **Profile Counter**: A live indicator always shows how many profiles
  are loaded and how many are currently checked (selected for operations).
- ✎ **Edit & Remove**: Click a profile row to select it. Edit button
  activates for a single selection; Remove button activates for one or more
  — delete multiple profiles at once with a single confirmation.
- 📂 **Open in File Explorer**: Double-click any profile row to open its
  folder in the system file manager (Windows Explorer, Finder, or
  xdg-open on Linux).

### Git Operations
All operations run **simultaneously** across all checked profiles in a
background thread, the interface stays fully responsive at all times.

- 📋 **Status** — `git status`
- 📜 **Log** — `git log`
- 🌿 **Branches** — `git branch`
- 🔍 **Diff** — `git diff`
- ⬇️ **Pull** — `git pull`
- ⬆️ **Push** — `git push`
- 🔄 **Fetch** / **Fetch All** — `git fetch` / `git fetch --all`
- ➕ **Stage All** — `git add -A`
- 💾 **Commit** — `git commit -m "..."`
- 🚀 **Stage, Commit & Push** — stages → commits → pushes in one click
- ⚡ **Pull → Stage → Commit → Push** — full sync cycle in one click
- 📌 **Stash** / **Stash Pop** / **Stash List**
- 📥 **Clone Repository** — clone any remote repository with optional
  branch, depth, and submodule options
- ➕ **Submodule Add** — add a remote repository as a submodule with
  optional sub-path, SSH passphrase support, and ghost-state detection
- ➖ **Submodule Remove** — full 7-step clean removal (deinit, index
  cleanup, directory removal, .gitmodules update)

### Commit Messages
- ⏱ **Auto date/time**: If the message field is left empty, the current
  timestamp is used as the commit message automatically.
- ✏️ **Custom messages**: Type any commit message before running Stage,
  Commit, or combined operations.

### Authentication
- 🔑 **SSH Passphrase**: A dialog appears when SSH authentication is
  required. The passphrase is optionally saved per profile (Base64-encoded).
  Wrong passphrases trigger a re-prompt automatically.
- 🔐 **HTTPS Credentials**: Username and token/password dialogs appear
  when required for HTTPS remotes, with optional per-profile storage.
- 🔄 **Auto-reuse**: Saved credentials are reused across operations without
  re-prompting.
- 🛡 **Auto upstream fix**: If a push fails because no upstream branch is
  set, AGm automatically sets it with `--set-upstream` and retries.

### Output Log
- 🎨 **Colour-coded output**:
  - Gold, operation name header
  - Blue (`#89dcff`) — untracked file paths
  - Green (`#40c057`) — staged changes (committed to index)
  - Red (`#f38ba8`) — unstaged modifications and errors
  - Orange, warnings
- 🔎 **Zoom**: Ctrl++ / Ctrl+- / Ctrl+wheel to resize log text.
- ↕ **Line spacing**: Adjustable via slider in Settings.
- 🔤 **Font**: Choose any installed font in Settings → Output Log.
- 🗑 **Clear Log**: Dedicated button below the Stash row (Ctrl+L).

### CLI Window (AGm | CLI)
An interactive terminal-style window for typing git commands manually.

- 💻 **Per-repository tabs**: Each checked profile opens as a separate tab.
  Multiple repos can be open simultaneously.
- 🎨 **Git status colours**: Output from `git status` is automatically
  colour-coded (untracked = blue, staged = green, unstaged = red) —
  same colours as the main output log.
- ⌨️ **Tab autocomplete**: Press Tab to complete from 30+ built-in git
  command suggestions. Matching is case-insensitive and contains-based.
- ⬆️ **History navigation**: ↑ / ↓ arrow keys navigate command history.
- 🔍 **Zoom**: Ctrl+scroll or Ctrl+± to resize terminal text.
- 🧹 **Clear**: Ctrl+L, or type `clear` / `cls`.
- 🔗 **Always focused**: Clicking anywhere in the CLI window (including the
  output area) immediately focuses the input field.

### Submodule Management
- ➕ **Add Submodule**: Enter SSH URL, optional sub-path (with folder
  browser), submodule name, and optional passphrase. On success, AGm offers
  to register the new submodule as an AGm profile.
- 🧹 **Ghost state recovery**: If a previous failed removal left index/config
  entries behind, AGm detects the "already exists in the index" error,
  warns the user, runs a full automatic cleanup, and retries the add.
- ➖ **Remove Submodule**: Lists all submodules from `.gitmodules` in a
  resizable table (with search). On confirmation, runs all 7 cleanup steps:
  remove from `.gitmodules`, stage, remove from `.git/config`, deinit,
  delete `.git/modules/` entry, delete the working directory, remove from
  the git index. On success, the matching AGm profile is removed
  automatically.

### Clone Repository
- 📥 **Clone dialog**: SSH Address, Destination Path (with browser),
  Repository Name, optional Branch, optional Depth, and an All Submodules
  checkbox (`--recurse-submodules`).
- 🔑 **SSH passphrase**: Optional field in the dialog; if omitted and SSH
  authentication fails, AGm prompts automatically and retries.
- 🚫 **Duplicate name guard**: The Repository Name field turns red in
  real-time if a profile with that name already exists.
- ➕ **Add as profile**: On successful clone, AGm offers to add the
  cloned repository as a new profile.

### Configuration
- 💾 **Auto-save**: Configuration is saved automatically to
  `~/.agm/agmconf` (Base64-encoded JSON). The config folder is hidden on
  Windows.
- 📂 **Load / Save / Save As**: Load any `.agm` config file; save the
  current state to any location.
- 🔄 **Reset**: Reset config path or wipe all settings back to defaults.
- ⚙️ **Settings dialog** (Help → Settings):
  - **Output Log tab**: font family, text size, line spacing, live preview
  - **CLI tab**: terminal background colour, text colour, tab name
    background, font size, window opacity, status line colours
    (untracked / staged / unstaged), Reset to Default button

---

## System Requirements

- **Operating System**: Windows 10 or later (recommended)
- **Git**: Git must be installed and available on the system `PATH`.
  Download from [https://git-scm.com](https://git-scm.com)
- No Python installation required, AGm ships as a standalone `.exe`.

---

## Usage

### 1. Launch AGm
Double-click `AGm.exe`. The main window opens with your profiles loaded
from the last session (if any).

### 2. Add Repository Profiles
Click **＋ Add** to add a single repository, or **📂 Import Folders…** to
import several at once. Each valid Git repository is added as a named
profile.

### 3. Select Profiles for Operations
Tick the checkbox of every repository you want to run an operation on.
Use **All** to check all, **None** to uncheck all, or **Ctrl+A** as a
keyboard shortcut. The counter at the bottom of the list shows how many
are checked.

### 4. Run a Git Operation
Click any operation button on the right panel (Status, Pull, Push, Stage,
Commit, etc.). Output appears live in the log below. The **Stop** button
(or **Esc**) cancels a running operation at any time.

### 5. Use the CLI Window
Check exactly the repositories you want, then click **💻 CLI**. A tab opens
for each selected repository. Type git commands directly and press Enter.
Open additional repos by checking them and clicking CLI again, each gets
its own tab.

### 6. Clone a Repository
Click **📥 Clone Repository…**, fill in the SSH address, destination folder,
and name, then click **Clone**. AGm handles SSH authentication and offers to
add the result as a profile.

### 7. Manage Submodules
Select a single profile and click **➕ Submodule Add** or **➖ Submodule
Remove**. The Remove dialog lists all submodules with a search field, select
one and confirm to run the full cleanup sequence automatically.

### 8. Adjust Appearance
Open **Help → Settings** to customise the output log font and the CLI
terminal colours. All changes are saved to config and persist across sessions.

---

## Keyboard Shortcuts

### Main Window
| Shortcut | Action |
|---|---|
| **Ctrl+A** | Check all profile checkboxes |
| **Ctrl+Q** | Quit AGm |
| **Ctrl+L** | Clear the output log |
| **Ctrl++  /  Ctrl+-** | Zoom output log text in / out |
| **Ctrl+Wheel** | Zoom output log with mouse scroll |
| **Esc** | Stop the currently running operation |
| **Double-click** profile | Open repository folder in file manager |

### CLI Window
| Shortcut | Action |
|---|---|
| **Ctrl+W** | Close the current tab |
| **Ctrl+1 … Ctrl+9** | Switch to tab 1 … 9 |
| **Ctrl+L** | Clear the current terminal |
| **Ctrl++  /  Ctrl+-** | Zoom terminal text in / out |
| **Ctrl+Wheel** | Zoom terminal with mouse scroll |
| **Tab** | Autocomplete the current git command |
| **↑ / ↓** | Navigate command history |
| Type **clear** or **cls** | Clear terminal output |

---

## Common Issues

- ❌ **Permission denied (publickey)**: Your SSH key is not authorised for
  the remote repository, or the passphrase entered was incorrect. Verify
  your SSH key is added to the remote (e.g. GitHub → Settings → SSH keys)
  and enter the correct passphrase when prompted.
- 🔄 **"Already exists in the index"**: A previous submodule add or remove
  failed and left ghost state. AGm detects this automatically and offers to
  clean up and retry.
- 📂 **Path not found** when opening CLI: The repository directory was moved
  or deleted. Update the profile path via the Edit button.
- ⏳ **Slow status colours on startup**: AGm checks `git status --porcelain`
  for every profile in the background. On slow drives or with many profiles,
  this may take a few seconds. The interface is fully usable while this runs.
- ⚙️ **No Git found**: Ensure Git is installed and `git --version` works in
  a terminal. On Windows, ensure "Git for Windows" is installed and its
  `bin` folder is on the PATH, or reinstall with the "Add to PATH" option.
- 🔒 **SSL / HTTPS error on push or pull**: If your network intercepts HTTPS
  traffic through a proxy, configure Git's proxy settings:
  `git config --global http.proxy http://your.proxy:port`

---

## Technical Notes

- AGm runs `git` as an external process, it uses whatever Git version is
  installed on the system.
- All git operations run in **background threads**; the GUI never freezes.
- SSH authentication uses the `SSH_ASKPASS` mechanism, AGm never opens a
  terminal window for passphrase prompts.
- The configuration file at `~/.agm/agmconf` is Base64-encoded JSON. It is
  **not encrypted**. Store the file in a secure location if it contains
  saved credentials.
- Submodule operations (add and remove) follow the standard Git submodule
  lifecycle and stage `.gitmodules` changes. A final `git commit` is needed
  after any submodule modification to record it in the parent repository.
- AGm supports both standard Git repos (`.git/` directory) and submodule
  repos (`.git` file pointer).

---

## Git / Hosting Provider Disclaimer

AGm is an **independent tool** and is **not affiliated with, endorsed by,
or associated with** GitHub, Inc., GitLab Inc., Atlassian Pty Ltd.,
Microsoft Corporation, or any other Git hosting provider in any way.

"GitHub", "GitLab", "Bitbucket", and "Git" are trademarks or registered
trademarks of their respective owners.

---

## License

This software is released as **freeware** under the **Avarwand EULA**.

By using AGm you agree to:
- Use the software in compliance with the EULA
- Not reverse engineer, decompile, or modify the software
- Not redistribute or claim ownership of the software
- Accept the software "as is" without warranties

*For full license terms, see the `LICENSE.txt` file.*

---

## Contact & Support

**Avarwand**
📧 Email: [avarwand@yahoo.com](mailto:avarwand@yahoo.com)
🐙 GitHub: [github.com/avarwand](https://github.com/avarwand)

---

**Developed by Avarwand**
**Initial Release: 2026 May**

---

© 2026 Avarwand. All rights reserved.