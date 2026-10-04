<div align="center">

Avarwand

# Git Manager

**End-User License Agreement (EULA) — Freeware**

</div>

This End-User License Agreement ("Agreement") is a legal agreement between you (an individual or an organisation, "you") and **Avarwand Software** ("Avarwand", "we") for **AGm — Avarwand Git Manager**, including the executable, the source script, the icons, the documentation and any updates provided by Avarwand (together, the "Software").

By installing, copying or using the Software you agree to this Agreement. If you do not agree, do not install or use the Software.

## 1. Freeware License

AGm is **freeware**. Avarwand grants you a free, non-exclusive, worldwide, non-transferable license to install and use any number of copies of the Software for **personal and commercial purposes**, including inside companies, schools and public organisations.

No registration, license key or payment is required.

## 2. Redistribution

You may redistribute the Software free of charge, provided that:

* it is distributed **unmodified** and complete, including this LICENSE file;
* all copyright notices, the name "AGm" and the Avarwand branding remain intact;
* **no fee** is charged for the Software itself (a reasonable charge for physical media or for a bundle in which AGm is only one free part is permitted);
* it is not presented as your own product, and no endorsement by Avarwand is implied;
* it is not bundled with malware, adware or any software that installs without the user's consent.

Distribution through package managers and software repositories (for example **WinGet**) and on mirror or download sites is permitted under these conditions.

## 3. Restrictions

Except where section 5 or applicable law expressly allows it, you may not:

* sell, rent, lease or sublicense the Software;
* distribute modified versions of the Software under the name "AGm" or "Avarwand";
* remove or alter any copyright notice, license text or branding;
* use the name "Avarwand" or "AGm" to promote other products without written permission.

## 4. Ownership

The Software is licensed, not sold. Avarwand retains all rights, title and interest in the Software, including copyright and all other intellectual property rights. All rights not expressly granted in this Agreement are reserved.

## 5. Third-Party Components

The Software uses or works with third-party components that remain the property of their respective owners and are licensed under their own terms:

| Component | Owner | License |
|---|---|---|
| PyQt5 (bundled in the EXE) | Riverbank Computing Ltd. | GNU GPL v3 or Riverbank commercial license |
| Qt 5 libraries (bundled in the EXE) | The Qt Company Ltd. | GNU LGPL v3 |
| Python runtime (bundled in the EXE) | Python Software Foundation | PSF License |
| Git (not included, installed by the user) | Git project | GNU GPL v2 |
| OpenSSH (not included, part of Windows or installed by the user) | OpenBSD project / Microsoft | BSD-style |

Nothing in this Agreement limits any rights you have under the license of a third-party component. Where a third-party license grants you rights that conflict with this Agreement, that license prevails for that component.

## 6. Your Data, Credentials and Privacy

* **No data collection.** AGm does not contain telemetry, analytics or advertising and does not send any information to Avarwand.
* **Network access.** AGm connects only to the Git servers (for example GitHub or GitLab) that you configure, using Git and OpenSSH on your computer. When AGm is run as a Python script, it may download missing dependencies (PyQt5) from the Python Package Index.
* **Local storage.** Profiles and settings are stored locally in `%USERPROFILE%\.agm\agmconf` (or in a configuration file you choose).
* **Saved credentials.** If you choose to save HTTPS usernames, passwords or SSH key passphrases, they are stored in that file in **encoded (Base64) form, not encrypted**. Anyone with access to your user account or to that file can read them. You are responsible for protecting your computer and the configuration file. Using SSH keys or access tokens with limited permissions is recommended.

## 7. Responsibility for Git Operations

AGm runs real Git commands on your repositories. Some operations can permanently change or delete data, including `git reset --hard`, `git push`, `git stash`, submodule removal and actions applied to several repositories at once.

You are solely responsible for the operations you start, for reviewing confirmation dialogs, and for keeping **backups** of your repositories and data.

## 8. No Warranty

The Software is provided **"as is" and "as available"**, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, non-infringement, uninterrupted operation and freedom from errors. You use the Software at your own risk.

## 9. Limitation of Liability

To the maximum extent permitted by applicable law, Avarwand shall not be liable for any direct, indirect, incidental, special or consequential damages, including loss of data, loss of source code, lost profits, business interruption or damage to repositories or remote accounts, arising from the use of or inability to use the Software, even if advised of the possibility of such damages.

Nothing in this Agreement excludes or limits liability that cannot be excluded or limited under applicable law, such as liability for intent or gross negligence, or for injury to life, body or health.

## 10. Updates

Avarwand may release updates, but is not obliged to provide updates, support or maintenance. Updates are licensed under the version of this Agreement included with them, unless they come with a different license.

## 11. Termination

This license ends automatically if you breach any of its terms. On termination you must stop using and distributing the Software and delete all copies in your possession. Sections 4 to 9 remain in effect after termination.

## 12. Severability

If any provision of this Agreement is held invalid or unenforceable, the remaining provisions remain in full force, and the invalid provision shall be replaced by a valid one that comes closest to its intended purpose.

## Contact

**Avarwand Software**

📧 [avarwand@yahoo.com](mailto:avarwand@yahoo.com)

🌐 https://github.com/avarwand/

---

© 2026 Avarwand. All rights reserved.
