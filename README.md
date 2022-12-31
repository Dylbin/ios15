# Jailbreaking iOS 15 and higher

Jailbreaking iOS 15 and higher is a more difficult task because of the new sealed filesystem introduced, and various security hardening.


# palera1n's teams method
- The public released jailbreak called palera1n utilizes the checkm8 bootROM exploit used by checkra1n, however palera1n uses different methods to achieve a rootless semi-tethered jailbreak.

### How does it work?

- At the first run it'll boot a ramdisk which dumps your onboard SHSH blob, creates a fakefs, installs a loader app and patches the kernel

- fakefs only gets created if using semi-tethered mode, disadvantage with semi-tethered mode is that the jailbreak will be rootless.
