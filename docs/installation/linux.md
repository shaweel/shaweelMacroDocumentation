# Installation on GNU+Linux
There are multiple ways to install shaweelMacro on [GNU+Linux](https://kernel.org). Ranging from distro-specific to completely universal.

Navigation:  
[Jump to Debian](#debian)  
[Jump to Fedora](#fedora)  
[Jump to the AUR](#the-arch-user-repository)  
[Jump to Flatpak](#flatpak)  
[Jump to .jar](#jar-file)
## Debian
For [Debian](https://www.debian.org) and its [derivatives](https://www.debian.org/derivatives/) you can install shaweelMacro by downloading a .deb file from the [latest release](https://github.com/shaweel/shaweelMacro/releases/latest) and installing it with `sudo apt install ./shaweelMacro.deb`

## Fedora
For [Fedora](https://fedoraproject.org) and its [derivatives](https://fedoraproject.org/wiki/Derived_distributions) you can install shaweelMacro by downloading a .rpm file from the [latest release](https://github.com/shaweel/shaweelMacro/releases/latest) and installing it with `sudo dnf install ./shaweelMacro.rpm`

## The Arch User Repository
For [Arch Linux](https://archlinux.org) and its [derivatives](https://wiki.archlinux.org/title/Arch-based_distributions) you can install shaweelMacro using [The Arch User Repository](https://aur.archlinux.org).

To install shaweelMacro, install the `shaweelMacro` package either with an [AUR helper](https://wiki.archlinux.org/title/AUR_helpers) like `yay` or `paru`  
`yay -S shaweelMacro` or  `paru -S shaweelMacro`  
or manually installing the package using `git` and `makepkg`  
`git clone https://aur.archlinux.org/shaweelMacro.git`  
`cd shaweelMacro`  
`makepkg -si`

## Flatpak
shaweelMacro can also be installed using `flatpak` on any distribution supporting it. This is generally not recommended if your distribution already has a native way of installing shaweelMacro

To install shaweelMacro via `flatpak` download a .flatpak file from the [latest release](https://github.com/shaweel/shaweelMacro/releases/latest) and install it with `flatpak install ./shaweelMacro.flatpak`

I am trying to get shaweelMacro on [Flathub](https://flathub.org/) as soon as possible.

## .jar file
You can also choose the universal option, which will run on anything which runs [Java](https://www.java.com/)

To run shaweelMacro using the .jar file, you will first have to ensure you have the Java 25 JRE or JDK installed. I recommend using [Adoptium Temurin JRE](https://adoptium.net/temurin/releases).

After making sure you have the Java 25 JRE or JDK installed, you can download a .jar file from the [latest release](https://github.com/shaweel/shaweelMacro/releases/latest) and simply run it with `java -jar ./shaweelMacro.jar` or on some [Desktop Environments](https://wiki.archlinux.org/title/Desktop_environment) just opening the file.