# Fix '/dev/sdxx: UNEXPECTED INCONSISTENCY; RUN fsck MANUALLY.'

1. Run `fsck` in the dropped down shell
```bash
fsch -y /dev/sdxx
```
2. Reboot the system
```bash
reboot -f
```

Tags:
```
#filesystem #inconsistancy #fsck
```

Related:
```
* https://askubuntu.com/questions/885062/root-file-system-requires-manual-fsck
* https://medium.com/@valmircsjr/solu%C3%A7%C3%A3o-linux-the-root-filesystem-on-dev-sdxx-requires-a-manual-fsck-38f0685efdd5
* https://deeptalk.lambdalabs.com/t/boot-hangs-with-the-root-file-system-on-dev-sda2-requires-a-manual-fsck/350
```
