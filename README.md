# My Web 🌐

Welcome to the **My Web**.

This project involves setting up and administering virtual machines as per the ASR company's requirements.

## Project Overview 🔎

You are tasked with creating two virtual machines:

1. **Client Machine (`my-client_${name}`):**
   - Dual Boot: Archlinux and Debian
   - Configuration: Free to define RAM and virtual hard drive size
   - Network: Bridged interface

2. **Server Machine (`my-web_${name}`):**
   - OS: Ubuntu Server (without a graphic environment)
   - Configuration: Free to define RAM and virtual hard drive size
   - Network: Bridged interface
   - Contains: HTTP server, database server, PHP module, database management application

## Client Machine Specifications

### Archlinux

- **Partitioning:**
  - 15 GB primary partition using LVM
  - Subpartitions: 9 GB root, 5 GB home, 400 MB boot, 500 MB swap
- **Graphic Environment:**
  - XFCE with a graphic session manager of choice
- **Locales:**
  - English language, keyboard in native language, and localization in your time zone
- **Users and Groups:**
  - User `leslie` in `adm` and `epitech` groups
  - User `romain` in `managers` and `epitech` groups, with `sudo` privileges
- **OS Access:**
  - Debian's `/home` accessible in Archlinux
- **SSH Server:**
  - Installed and listening on port 42

### Debian

- **Partitioning:**
  - 10 GB root, 4.5 GB home, 500 MB boot, 500 MB swap
- **Graphic Environment:**
  - Cinnamon
- **Locales:**
  - French language, keyboard, and Shanghai localization
- **Users and Groups:**
  - Users `hadrien`, `vincent` (in `pedago` and `epitech`), and `luc` (in `students` and `epitech`)
  - Cross command execution permissions for `hadrien` and `vincent`
- **SSH Server:**
  - Installed and listening on port 42

## Server Machine Specifications

- **Web Server:**
  - Setup with HTTP server, database server, PHP module, and database management application
  - Two intranet sites: `intra.asrlab.lan` and `intra-adm.asrlab.lan`
- **SSH Server:**
  - Installed and listening on port 42

## Installation and Setup Instructions 💾

### Dual Boot VM Setup

Refer to [Dual Boot VM Setup Guide](https://www.youtube.com/watch?v=Yn91wf9KyqY) for detailed instructions.

### VirtualBox Installation

```shell
sudo su
dnf install VirtualBox
akmods && systemctl restart systemd-modules-load.service
VirtualBox
```
Archlinux and Debian Setup
Follow the provided steps in the project notes to configure both Archlinux and Debian operating systems within the virtual machine.

For detailed guidelines, refer to `my-web.pdf`.

Embark on this virtual machine administration journey and hone your system administration skills!

## License ⚖️

This project is released under the MIT License. See `LICENSE` for more details.
