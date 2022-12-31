# Jailbreaking iOS 15 and higher

Jailbreaking iOS 15 and higher is a more difficult task because of the new sealed filesystem introduced, and various security hardening.


# palera1n's teams method
- The public released jailbreak called palera1n utilizes the checkm8 bootROM exploit used by checkra1n, however palera1n uses different methods to achieve a rootless semi-tethered jailbreak.

### How does it work?

- At the first run it'll boot a ramdisk which dumps your onboard SHSH blob, creates a fakefs, installs a loader app and patches the kernel

- fakefs only gets created if using semi-tethered mode, disadvantage with semi-tethered mode is that the jailbreak will be rootless.

- Running the jailbreak in tethered mode skips the fakefs, renames your normal fs so it doesn't reset on reboots, iOS 15 prevents this but utilizing checkm8 we can boot a dev kernel tethered.

### Issues with A10 and A11 devices

- Passcode must be disabled before jailbreaking or entering a jailbroken state.

- On iOS 16 this is even more strict. If you EVER enabled a passcode on iOS 16 you have to reset the entire device before proceeding.
