# Extend LVM

1. Create Physical volume
```bash
pvcreate /dev/sdXX
```

2. Extend volume group
```bash
vgextend <vg-name> /dev/sdXX
```

2. Extend logical volume
```bash
lvextend -L +<size>[T,G] <lvpath>
```

Tags:
```
#lvm #extend
```

