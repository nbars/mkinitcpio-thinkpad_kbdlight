# mkinitcpio-thinkpad_kbdlight
This hook can be used to turn the keyboard backlight on when entering initrd. On leaving initrd, the backlight is switched off again.

Move files into `/etc/initcpio` and add the hook to the `HOOKS` list e.g.
```
HOOKS="base udev autodetect modconf block filesystems keyboard thinkpad_kbdlight keymap encrypt fsck"
```
Rebuild initrd:
```
mkinitcpio -p linux
```
