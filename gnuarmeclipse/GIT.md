## Repository URLs

- the GNU ARM Eclipse git remote URL to clone from is **ssh://ilg-ul@git.code.sf.net/p/gnuarmeclipse/qemu**
- the QEMU git remote URL is **git://git.qemu-project.org/qemu.git**.

Add a remote named *qemu*, and pull its master → master.

## Update procedures

### The gnuarmeclipse-dev branch

To keep the development repository in sync with the original QEMU repository:

- checkout master
- pull from qemu master
- checkout gnuarmeclipse-dev
- merge master
- add a tag like gae-2.3.0-201403261500-dev after each public release

### The gnuarmeclipse branch

To keep the stable development in sync with the development branch:

- checkout gnuarmeclipse
- merge gnuarmeclipse-dev
- add a tag like gae-2.3.0-201403261500 after each public release




