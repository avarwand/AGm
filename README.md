<div align="center">

Avarwand

# Git manager

</div>

**AGm** is a modern Windows GUI tool for managing many Git repositories at the same time. Tick the repositories you want, click one button, and AGm runs the operation on all of them, one after the other.

It lets you check, commit, and synchronise your projects quickly, without the command line and without typing the same Git commands in folder after folder.

## Features

* **Profiles**: Add repositories one by one or import many folders at once. Live colours show which repositories are clean and which have changes. Search and filters help you find them quickly.
* **Batch Operations**: Status, Branches, Log, Blame, Pull, Push, Fetch, Stage, Commit, and Stash for all ticked repositories with one click, including complete workflows such as Stage, Commit and Push.
* **Smart Submodule Handling**: Submodules are committed and pushed before their main repository, so the main project always records the newest state. Submodules can be added and removed cleanly.
* **Safety Checks**: Files that are too large for GitHub are reported before every push, and risky actions such as Reset or Stash Pop ask for confirmation first.
* **History Tools**: A coloured diff viewer with line numbers and search, release tags, and a safe Git Reset that shows what will change before it happens.
* **Clone**: Clone repositories over SSH or HTTPS with branch, depth, and submodules, and add them as profiles right away.
* **SSH and Credentials**: An SSH Setup Assistant guides you through setting up SSH on a new computer. A key manager creates, imports, and manages SSH keys. Passwords and passphrases are asked for in AGm's own windows.
* **Git Identity**: See all Git identities on the computer, and set, edit, or remove them globally or for a single repository.
* **More Tools**: An auto-commit timer, a built-in CLI window with one tab per repository, a live progress bar, and a searchable built-in manual.
* **Modern GUI**: Clean interface with colour-coded status information that adapts to large monitors and small laptop screens. No command-line knowledge required.

## System Requirements

* Windows 10 or Windows 11
* [Git for Windows](https://git-scm.com/download/win)
* OpenSSH client (included in Windows 10 and 11) for SSH connections
* Administrator rights are not required; they are only asked for when the SSH Setup Assistant installs OpenSSH or enables the ssh-agent service

## Installation

Download the latest installer (MSI) from the [GitHub Releases](https://github.com/avarwand/AGm/releases) page and run it.

If Git is not installed yet, AGm shows this at the bottom right of the main window together with a link to the Git for Windows download page.

## Good to Know

* **Saved credentials**: Passwords, tokens, and SSH passphrases are only saved if you choose "Remember". They are stored encoded, not encrypted, in AGm's configuration file in your user folder. You can remove them at any time in the profile settings.
* **One global Git identity**: Git allows only one global user per computer. Repositories can have their own identity, which overrides the global one.
* **exFAT and FAT32 drives**: Repositories on drives that do not record file ownership are handled automatically by AGm.
* **Updates**: AGm can check for new versions on request or automatically at startup. Nothing is downloaded or installed automatically.

## Use Cases

AGm can be useful for:

* Committing and pushing all your projects at the end of the day with one click
* Keeping many repositories and their submodules up to date
* Reviewing changes between commits and undoing mistakes
* Preparing releases with tags
* Setting up SSH for Git on a new computer
* Working with different Git identities for private and work projects
* Avoiding failed pushes caused by very large files
* General software development and maintenance tasks

## Freeware

AGm is released as **freeware** by **Avarwand Software**.

You may use AGm free of charge for personal and commercial purposes. Redistribution is permitted under the terms of the included EULA.

For complete licensing terms, see [LICENSE.md](LICENSE.md).

---

## About

**Developed by Avarwand Software**

**Initial Release:** May 2026 <br> 
**Latest Update:** November 2026 (v1.5.2.1)



📧 [avarwand@yahoo.com](mailto:avarwand@yahoo.com)  
🌐 [github.com/avarwand](https://github.com/avarwand/)

© 2026 Avarwand. All rights reserved.
