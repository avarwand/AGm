# End User License Agreement (EULA)

## AGm (Avarwand Git manager)


This End User License Agreement (the "Agreement") is a legal agreement between you, either an individual or a legal entity ("You"), and **Avarwand** (independent software developer, the "Author") for the software product **"Avarwand Git manager"** ("AGm" or the "Software"), including its executable files and any accompanying documentation.

The Software is a **freeware** tool for managing multiple Git repositories from one window: batch Git operations (status, pull, push, fetch, stage, commit, stash), tags, diffs, resets, cloning, submodules, SSH key setup and management, and Git identity settings. It is distributed in compiled executable form only, as a Windows installer (MSI). The source code is not published.

**By installing, copying, or otherwise using the Software, You agree to be bound by the terms of this Agreement. If You do not agree to these terms, do not install or use the Software.**

---

### 1. License Grant

The Author grants You a non-exclusive, worldwide, royalty-free license to install and use the Software, free of charge, on any number of devices, for both personal and commercial purposes, subject to the terms of this Agreement.

The Software is licensed, not sold.

---

### 2. Free Redistribution and Promotion

The Author welcomes the free sharing of the Software. Any person, organization, or platform may redistribute, host, mirror, advertise, and promote the Software **free of charge**, provided that all of the following conditions are met:

1. **Unmodified and complete.** The Software is distributed in its original, complete, and unmodified form, including this Agreement and all copyright and proprietary notices.
2. **No monetization.** No fee, payment, donation, or other compensation may be charged or required for the Software, or for access to, downloading, or redistribution of it, whether directly or indirectly (for example, through a paid membership, package, or subscription that includes the Software). The Software may not be sold, rented, leased, sublicensed for compensation, offered as a paid download, used as a purchase incentive or reward, or bundled with or tied to any paid product, service, or subscription.
3. **Free and unrestricted access.** Where the Software is made available to the public, access to it may not be conditioned on any barrier or obligation, including mandatory registration or account creation, completion of surveys or third-party offers, provision of payment details, "content lockers" or similar unlock mechanisms, or artificial waiting periods, speed limits, or download limits designed to promote a paid service. The Software must remain directly and freely accessible to all end users.
4. **Honest attribution.** The Software must be clearly attributed to Avarwand. You must not claim ownership or authorship of the Software or present it as your own work.
5. **No deceptive or harmful distribution.** The Software must not be distributed together with malware, adware, or unwanted bundled software, nor through deceptive "download wrappers," pay-per-install installers, or similar schemes.

Ordinary advertising on a hosting or promoting platform (for example, an ad-supported download website or a monetized video review) is permitted, provided that the Software itself remains free of charge and that the advertising does not gate or condition access to it (see condition 3 above).

Where reasonably possible, please link to the official source: [github.com/avarwand](https://github.com/avarwand/)

---

### 3. Restrictions

Except as expressly permitted in this Agreement, You will not, and will not permit others to:

1. Reverse engineer, decompile, or disassemble the Software, or attempt to derive its source code, **except and only to the extent that such activity is expressly permitted by applicable law notwithstanding this limitation** (for example, under Articles 5 and 6 of Directive 2009/24/EC or §§ 69d and 69e of the German Copyright Act) **or by the license terms of an included third-party component**;
2. Modify, adapt, translate, or create derivative works of the Software;
3. Remove, alter, or obscure any copyright, trademark, or other proprietary notices;
4. Sell, rent, lease, sublicense, or otherwise commercially exploit the Software;
5. Use the Software for any unlawful, malicious, or harmful purpose.

---

### 4. Acceptable Use

The Software runs Git commands on the repositories You select. It can change local files and repository history, publish content to remote servers, and change Git and SSH settings of the device it runs on. You agree to use these functions responsibly and only where You are entitled to do so. In particular:

1. **Own or authorized repositories.** Use the Software only with repositories, remote servers, and accounts that You own or are authorized to use. Pushing, tagging, or rewriting history on repositories of others without permission may be unlawful or violate the terms of the hosting service.
2. **Organizational policies.** On devices, repositories, or accounts managed by an employer, school, or other organization, comply with that organization's policies, including policies on credentials, SSH keys, and source code.
3. **Credentials and keys.** The Software can store passwords, access tokens, and SSH key passphrases on Your device (only if You choose "Remember"), and it can create, import, rename, and delete SSH keys. Stored credentials are encoded, not encrypted. Protect Your device and the Software's configuration files, and do not share them with unauthorized persons.

---

### 5. Ownership

All rights, title, and interest in and to the Software, including all intellectual property rights, are and shall remain the exclusive property of the Author. All rights not expressly granted to You in this Agreement are reserved by the Author.
The AGm icon and branding elements are original creations of Avarwand.

---

### 6. Name and Trademarks

"Avarwand", "Avarwand Git manager", "AGm", and any associated logos identify the Author and the Software. This Agreement does not grant You any right to use these names or logos as Your own trademarks, brand names, product names, or product identities.

You may use these names solely to truthfully identify, describe, and promote unmodified copies of the Software, provided that such use does not suggest sponsorship, endorsement, or affiliation by the Author and is not likely to cause confusion.

"Git" is a trademark of the Software Freedom Conservancy. "GitHub", "GitLab", "Bitbucket", "Microsoft", "Windows", and other product names mentioned in the Software or its documentation are trademarks of their respective owners. The Software is an independent product and is not affiliated with, endorsed by, or sponsored by any of these owners.

---

### 7. Third-Party Components

The Software may include third-party components (such as open-source libraries) that are subject to their own license terms. Those terms apply to the respective components and, in the event of a conflict, take precedence over this Agreement for those components. Any applicable third-party notices are provided in an accompanying `THIRD-PARTY-NOTICES` file.

The Software requires **Git for Windows**, and for SSH connections the **OpenSSH client**. These programs are not part of the Software, are installed separately, and are subject to their own license terms.

---

### 8. Privacy

The Software runs locally on Your device. The Author does not collect, store, or receive any personal data, usage statistics, or telemetry.

Some functions contact services on the internet when You use them:

* **Git operations** (pull, push, fetch, clone, and similar): Git connects to the remote servers that You have configured for Your repositories (for example, GitHub or GitLab) and transmits Your repository data and credentials to them.
* **Update check**: when You click "Check for Updates", or if You have enabled the automatic check, the Software asks the GitHub API (api.github.com) for the latest published release of AGm. Only this request is sent; it contains the installed version number. Nothing is downloaded or installed automatically.
* **Links**: some buttons open web pages (for example, the SSH key settings on GitHub or GitLab, or the AGm releases page) in Your web browser.

These requests are sent directly from Your device to the respective service. As with any internet connection, these services receive Your public IP address; their own privacy policies apply. The results are only displayed on Your device and are not transmitted to the Author.

Profiles, settings, and any credentials You choose to remember are stored only on Your device, in the Software's configuration files in Your user folder.

---

### 9. Disclaimer of Warranty

To the maximum extent permitted by applicable law, the Software is provided **"AS IS"**, without warranty of any kind, either express or implied, including but not limited to the implied warranties of merchantability, fitness for a particular purpose, and non-infringement. The Author does not warrant that the Software will be error-free or uninterrupted.

You use the Software at Your own risk. In particular:

* **Data loss.** Some operations can permanently discard changes or files, for example a hard reset, popping a stash, removing a submodule, or deleting SSH keys. Make sure You understand an operation and have a backup before running it.
* **Published content.** A push sends Your commits, files, and tags to a remote server, where they may become visible to others. Check what You publish, especially passwords, keys, and other confidential data.
* **System and Git settings.** Changing Git settings (for example, Your Git identity or trusted repository folders), SSH settings, or the ssh-agent service affects other programs on Your device that use Git or SSH.

---

### 10. Limitation of Liability

To the maximum extent permitted by applicable law, in no event shall the Author be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, without limitation, loss of data, loss of source code or repository history, disclosure of confidential information, security incidents, system damage, loss of profits, or business interruption) arising out of the use of or inability to use the Software, even if advised of the possibility of such damages.

Nothing in this Agreement excludes or limits the Author's liability for willful misconduct or gross negligence, for injury to life, body, or health, or for any other liability that cannot be excluded or limited under applicable law. The mandatory statutory rights of consumers remain unaffected.

---

### 11. Termination

This Agreement is effective until terminated. Your rights under this Agreement will terminate automatically, without notice from the Author, if You fail to comply with any of its terms. Upon termination, You must immediately cease all use of the Software and destroy all copies in Your possession or control.

Sections 5, 6, 9, 10, 12, and 13 shall survive any termination of this Agreement.

---

### 12. Severability

If any provision of this Agreement is held to be invalid or unenforceable, that provision shall be enforced to the maximum extent permissible, and the remaining provisions of this Agreement shall remain in full force and effect.

---

### 13. Governing Law

This Agreement shall be governed by and construed in accordance with the laws of the Federal Republic of Germany, excluding its conflict-of-law rules and the United Nations Convention on Contracts for the International Sale of Goods (CISG).

If You are a consumer, this choice of law does not deprive You of the protection afforded to You by the mandatory provisions of the law of the country in which You habitually reside.

---

### 14. Entire Agreement

This Agreement constitutes the entire agreement between You and the Author with respect to the Software and supersedes all prior or contemporaneous communications and proposals regarding its subject matter.

---


**© 2026 Avarwand. All rights reserved.**

Contact: [avarwand@yahoo.com](mailto:avarwand@yahoo.com)

Official page: [github.com/avarwand](https://github.com/avarwand/)
