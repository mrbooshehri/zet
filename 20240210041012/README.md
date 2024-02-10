# SecureBoot status in Linux machine

To verify whether a Linux instance is enabled for UEFI Secure Boot
Run the following command as root on the instance.

``` bash
mokutil --sb-state 
```

Expected output:
- If UEFI Secure Boot is enabled, the output contains SecureBoot
	enabled.
- If UEFI Secure Boot is not enabled, the output contains SecureBoot
	disabled or Failed to read SecureBoot.

Tags:
```
#Linux #secureboot #secure #boot
```

Related:
```
* https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/verify-uefi-secure-boot.html
```
