# GNU ARM Eclipse QEMU

The [GNU ARM Eclipse QEMU](http://gnuarmeclipse.github.io/qemu) subproject is a fork of [QEMU](http://wiki.qemu.org/Main_Page) (an open source machine emulator), intended to provide support for Cortex-M emulation in GNU ARM Eclipse. The source code is part of the **GNU ARM Eclipse** project, and is available from [GitHub](https://github.com/gnuarmeclipse/qemu). Binary packages are available from [GitHub Releases](https://github.com/gnuarmeclipse/qemu/releases).

## How to use

* [Overview](http://gnuarmeclipse.github.io/qemu/) (read me first!)
* [QEMU Install](http://gnuarmeclipse.github.io/qemu/install)
* Eclipse plug-in
* [Support](https://github.com/gnuarmeclipse/qemu/issues/1) (using the GitHub Issues)

## How to build

Follow original "How to build" from QEMU with some **minor changes**
* [How to build](http://gnuarmeclipse.github.io/qemu/build-procedure) (using Docker containers)
* [Change log](http://gnuarmeclipse.github.io/qemu/change-log) ([2014](http://gnuarmeclipse.github.io/qemu/change-log/2014))

**minor changes:**

curl -L https://github.com/Jumperr-labs/build-scripts/raw/master/scripts/build-qemu.sh -o ~/Downloads/build-qemu.sh

## How to build with debug-symbols

After building:
```bash
#Remove all executables:

find ~/Work/qemu/ -name "qemu-system-gnuarmeclipse" | xargs -I{} rm "{}"

bash ~/Downloads/build-qemu.sh --all --no-strip
```
## Releases & binaries

See the [releases](http://gnuarmeclipse.github.io/qemu/releases) page.
Binaries for most platforms can be downloaded from [GitHub Releases](https://github.com/gnuarmeclipse/qemu/releases).
