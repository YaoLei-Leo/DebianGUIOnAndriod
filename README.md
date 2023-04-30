# DebianGUIOnAndriod
This repository is to record how to setup debian GUI on android system using Termux and Termux X11.

## Background
[Termux](https://termux.dev/en/) is a linux environment terminal emulator that developed for andriod system. It doesn't require root privilege and offers a lot of additional linux packages. It's system is very similar to linux's. Therefore, we can achieve many things with Termux. The full description of Termux can be found in [wikipedia](https://en.wikipedia.org/wiki/Termux#).

* [Termux X11](https://github.com/termux/termux-x11) is a Termux add-on app providing Android frontend for Xwayland. Termux X11 uses Wayland display protocol. a modern replacement and the predecessor of the X.org server.

[Chroot](https://en.wikipedia.org/wiki/Chroot) is a command on Unix and Unix-like operating systems. The chroot system call was introduced during development of Version 7 Unix in 1979. One source suggests that Bill Joy added it on 18 March 1982, 17 months before 4.2BSD was released, in order to test its installation and build system. Chroot is an operation that changes the apparent root directory for the current running process and its children. A program that is run in such a modified environment cannot name (and therefore normally cannot access) files outside the designated directory tree. This is usually done for security, containerization, or testing, and is often called a "chroor jail". Chroot can be used build up a container because it provides an isolated environment for running applications and can limit access to the rest of the file system. Therefore, we can build a linux system in Termux using chroot.

* [PRoot](https://wiki.termux.com/wiki/PRoot) is a user-space implementation of chroot, mount --bind, and binfmt_misc. This means that users don't need any privileges or setup to do things like using an arbitrary directory as the new root filesystem, making files accessible somewhere else in the filesystem hierarchy, or executing programs built for another CPU architecture transparently through QEMU user-mode.

  * [PRoot Distro](https://github.com/termux/proot-distro) is a Bash script wrapper for utility proot for easy management of chroot-based Linux distribution installations. It does not require root or any special ROM, kernel, etc. Everything you need to get started is the latest version of Termux application. PRoot Distro is not a virtual machine, neither a traditional chroot. It shares the same kernel as your Android system. PRoot supports many linux distributions, such as Alpine Linux (edge), Arch Linux/Arch Linux 32/Arch Linux ARM, Debian (stable),Ubuntu (22.04), etc.

