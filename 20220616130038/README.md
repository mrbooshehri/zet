# Install deb packages in arch Linux

* Install ```debtap``` package with an AUR helper
```bash
yay -S debtap
```
* Update ```debtap```
```bash
sudo debtap -u
```
* Convert your ```.deb``` package
```bash
deptab PACKAGE.deb
```
* Install converted package with ```pacman```
```bash
sudo pacman -U PACKAGE
```
Tags:
```
#arch #deb #deptap
```
Related:
```
* https://low-orbit.net/arch-linux-how-to-install-deb-package
```
