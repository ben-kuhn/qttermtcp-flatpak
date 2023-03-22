# qttermtcp-flatpak
Flatpak for G8BPQ's QtTermTCP


This application is not currently on FlatHub because I am not the author of QtTermTCP.  Once I have the bugs worked out I will approach John G8BPQ about submitting to FlatHub.

This flatpak has been tested and runs on amd64 and aarch64 systems.  It may run on others but it has not been tested.

build and install this flatpak you will need to do the following:

1.  Install Flatpak and configure FlatHub for your particular distribution.  See https://flatpak.org/setup/ for distro-specific instructions.
2.  Install flatpak-builder.  Use the same repository you used to install flatpak.
3.  Install the KDE SDK.

```install org.kde.Sdk//5.15-22.08```
4.  Install the KDE platform

```flatpak install org.kde.Platform//5.15-22.08```
5.  Clone the repo

```git clone https://github.com/ben-kuhn/qttermtcp-flatpak.git``
6.  Enter the directory

```cd qttermtcp-flatpak```
7.  Build and install the flatpak

```flatpak-builder --install --user --force-clean build-dir net.g8bpq.qttermtcp.yaml```
8.  Run the flatpak

```net.g8bpq.qttermtcp```
