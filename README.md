VPS2Arch
========

How To Use
---
```
wget https://raw.githubusercontent.com/Bryan2333/vps2arch/refs/heads/master/vps2arch

chmod +x vps2arch

./vps2arch
```

Changes
-------

This version changes the original script in the following ways.

Added:

- Interactive setup for SSH port, locale, timezone, DNS servers, hostname, SSH key login, BBR, `linux-zen`, custom mirrors, and swap file creation.
- Command-line options for the new setup fields: `-p`, `-l`, `-z`, `-d`, `-H`, `-k`, `-B`, and `-s`.
- Built-in default Arch mirrors and support for multiple custom mirrors.
- Support for current Arch bootstrap `.tar.zst` images.
- Locale, timezone, DNS, hostname, SSH, timesync, resolved, BBR, mirrorlist, and optional swap file configuration in the installed system.
- `linux-zen` kernel support.
- `bash-completion` installation and root skeleton file copying.

Removed:

- Country-based mirror discovery through the Arch mirrorlist API.
- Post-install mirror generation through `reflector`.
- `netctl` networking support.
- OpenVZ-specific support and compatibility workarounds.
- Backup and restore of the old system's hostname and localtime files.

Credits
-------

Original author: [Timothy Redaelli](mailto:timothy@fsfe.org)
