# Rescan disk Linux

```bash
for h in $(ls /sys/class/scsi_host); do
    echo '- - -' > /sys/class/scsi_host/$h/scan
done
```

Tags:
```
#scan #disk #linux
```
