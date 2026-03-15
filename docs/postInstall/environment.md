# Environment Type

Whenever you start shaweelMacro, it starts an isolated environment in which it starts [Sober](https://sober.vinegarhq.org/).

There are two options for which isolated environment shaweelMacro will launch. The first one is running with [Gamescope](https://github.com/ValveSoftware/gamescope), second is running inside a [QEMU](https://www.qemu.org/) [virtual machine](https://en.wikipedia.org/wiki/Virtual_machine). Below you can see pros and cons of both:

## Gamescope
[Gamescope](https://github.com/ValveSoftware/gamescope) is a [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) micro-compositor made by [Valve](https://www.valvesoftware.com/) for [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org). It runs a nested [Wayland](https://wayland.freedesktop.org/) compositor session on top of your current [desktop environment](https://wiki.archlinux.org/title/Desktop_environment).

### Pros:
- Very little performance impact—similar to simply running [Sober](https://sober.vinegarhq.org/) natively
### Cons:
- [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org) only—[Gamescope](https://github.com/ValveSoftware/gamescope) simply doesn't exist on [Windows](https://windows.com)
- Singleton—you cannot run another instance of [Sober](https://sober.vinegarhq.org/) while it's running

## QEMU Virtual Machine
[QEMU](https://www.qemu.org/) is a [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) virtualizer for [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org), [Windows](https://windows.com) and [MacOS](https://www.apple.com/os/macos/), allowing emulation of a whole [operating system](https://en.wikipedia.org/wiki/Operating_system).

In the context of shaweelMacro, QEMU sits as a middleman and helps create a [virtual machine](https://en.wikipedia.org/wiki/Virtual_machine) of a stripped down version of [Arch Linux](https://archlinux.org/) in which shaweelMacro continues.

### Pros:
- Works on both [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org) and [Windows](https://windows.com)
- Full isolation—allows for running [Roblox](https://roblox.com) on the [host operating system](https://www.geeksforgeeks.org/operating-systems/difference-between-host-and-guest-operating-system/).
### Cons:
- High performance impact—system resources must be allocated and the [guest operating system](https://www.geeksforgeeks.org/operating-systems/difference-between-host-and-guest-operating-system/) must use the [GPU](https://en.wikipedia.org/wiki/Graphics_processing_unit) in order for [Sober](https://sober.vinegarhq.org/) to run.
- Might cease to work on low-end machines

## Frequently asked questions

### Why not bypass the singleton?
1. [Roblox](https://roblox.com) considers this as malicious behaviour.
2. Because of this, [Sober](https://sober.vinegarhq.org/) *heavily* enforces this and will patch any bypass found, because they do not want to get on [Roblox](https://roblox.com)'s bad side, since [Roblox](https://roblox.com) doesn't support [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org) natively. Such bypass could obviously not be hidden because of the [free and open source](https://en.wikipedia.org/wiki/Free_and_open-source_software) nature of shaweelMacro.

### I'm on Windows, yet a virtual machine uses too many system resources for my PC to handle, what can I do?
Consider switching to [GNU](https://gnu.org/home.en.html)+[Linux](https://kernel.org)

### Why not add support for Windows Subsystem for Linux?
I considered it. It's too much of a hastle. I might add support for it in the future.