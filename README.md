# DebianGUIOnAndriod
This repository is to record how to setup debian GUI on android system using Termux and Termux X11.

## Background
[Termux](https://termux.dev/en/) is a linux environment terminal emulator that developed for andriod system. It doesn't require root privilege and offers a lot of additional linux packages. It's system is very similar to linux's. Therefore, we can achieve many things with Termux. 

[Chroot](https://en.wikipedia.org/wiki/Chroot) is a command on Unix and Unix-like operating systems. The chroot system call was introduced during development of Version 7 Unix in 1979. One source suggests that Bill Joy added it on 18 March 1982, 17 months before 4.2BSD was released, in order to test its installation and build system. Chroot is an operation that changes the apparent root directory for the current running process and its children. A program that is run in such a modified environment cannot name (and therefore normally cannot access) files outside the designated directory tree. This is usually done for security, containerization, or testing, and is often called a "chroor jail". Chroot can be used build up a container because it provides an isolated environment for running applications and can limit access to the rest of the file system.
