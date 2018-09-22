# mkinitcpio-thinkpad_kbdlight
Move files into `/etc/initcpio` and add the hook to the `HOOKS` list e.g.
```
HOOKS="base udev autodetect modconf block filesystems keyboard thinkpad_kbdlight keymap encrypt fsck"
```

You should take care of adding the hook, before the hook for that you actually need the illuminated
backlight.
