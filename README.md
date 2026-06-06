# Linux Installation and Basic Commands

When downloading Linux distributions, **amd64** usually means the 64-bit version, while **x86** refers to the 32-bit version.

In most cases, it is recommended to download the **x86_64** version because it supports 64-bit systems and can also run 32-bit applications.

When downloading ISO files, a **SHA-256 hash** is usually provided. You can use a SHA-256 calculator to verify the integrity of the downloaded file and make sure it has not been modified or corrupted.

Sometimes you will see the word **Live** in a Linux image. A Live version does not require installation. It can be booted directly from a USB flash drive or DVD and runs entirely from RAM. Live systems are useful for testing a distribution without installing it, and they are also widely used in areas such as digital forensics and data recovery.

### Common installation image types

* **Minimal:** Contains only the basic packages and has the smallest size.
* **DVD:** Includes most or all packages of the operating system.
* **Torrent:** Used for downloading the image through the BitTorrent protocol.
* **Checksum:** Contains the hash values used to verify the downloaded files.

## Creating a Bootable USB

One of the most popular tools for creating a bootable USB drive is **Rufus**.

## Installing Linux in VMware

When creating a new virtual machine and selecting the operating system type, VMware does not actually install that operating system. It simply adjusts the virtual hardware settings based on the recommended configuration.

## Linux Terminal Basics

Commands in Linux are entered through the **Terminal**.

If the prompt ends with a **$** symbol, it means you are logged in as a normal user.

If the prompt ends with a **#** symbol, it means you are logged in as the **root** user.

### Useful commands

* `ls` : Displays the files and directories in the current location.
* `cd` : Stands for **Change Directory** and is used to move between folders.
* `pwd` : Stands for **Print Working Directory** and shows your current location in the file system.
* `cat /etc/os-release` : Displays information about the installed Linux distribution and its version.

Linux terminals support **auto-completion**. For example, if you type the first few letters of a directory name and press the **Tab** key, the terminal will automatically complete it.

To execute commands with administrator privileges, use the `sudo` command before the actual command.

## Virtual Machine Snapshots

Taking a snapshot is useful before running suspicious files, malware samples, or any code that might damage the system. If something goes wrong, the virtual machine can be restored to its previous state.

## Installing WSL (Windows Subsystem for Linux)

Before installing WSL, it may be necessary to change the Windows region settings from Iran to the United States.

It is also recommended to use a VPN during the installation process.

The following Windows features should be enabled:

* Virtual Machine Platform
* Windows Subsystem for Linux (WSL)

After enabling them, restart the computer.

It is also a good idea to enable **Hyper-V** and **Containers** if they are available.

To install a Linux distribution in WSL, use:

```bash
wsl --install -d <distribution-name>
```

For example:

```bash
wsl --install -d kali-linux
```
