# Clone vagrant box
1. Export existing box
```bash
vagrant halt
vagrant package
```
2. Create a new directory and initial vagrant
```bash
mkdir duplicatedVM
cd duplicatedVM
vagrant init
```
3. Edit the new vagrant file and add the following lines
```bash
vim duplicatedVM/Vagrantfile
```
```bash
  config.vm.box = "any-name"
  config.vm.box_url = "file://PATH/TO/duplicatedVM/package.box"
  config.vm.network "public_network"
```
4. Start the VM
```bash
vagrant up
```

Tags:
```
#vagrant #clone #duplicate #vagrant_clone #vagrant_duplicate
```

Related:
```
* https://www.sparxsys.com/blog/how-copy-or-clone-vagrant-box
```

