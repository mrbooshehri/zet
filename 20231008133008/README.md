# How to LVM

1. Create physical volume
```bash
pvcreate </dev/sdx>
```

2. Create volume group
```bash
vgcreate <vg-name> </dev/sdx>
```

3. Create logical volume
```bash
lvcreate -l <Free  PE> -n lv0 vg0
```

> **Note:** You can get `Free  PE` from `vgdisplay`

4. Format disk
```bash
mkfs.ext4 </dev/VG_NAME/LV_NAME> 
```

5. Add it to `fstab`
6. Mount to desire mount point
```bash
mount -a
```

Tags:
```
#lvm #linux
```
