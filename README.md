# xkb-us-umlaut-capslock

Disables the standard capslock function and uses capslock german Umlauts:

 - CapsLock + a = ä
 - CapsLock + u = ü
 - CapsLock + o = ö
 - CapsLock + Shift + A = Ä
 - CapsLock + Shift + U = Ü
 - CapsLock + Shift + O = Ö
 - CapsLock + s = ß
 - CpasLock + e = €

## Installation 

```
# clone repo
git clone https://github.com/Bouni/xkb-us-umlaut-capslock

# enter cloned repo
cd xkb-us-umlaut-capslock

# copy keymap file
sudo cp usde /usr/share/X11/xkb/symbols/usde

# set keymap file
setxkbmap -model pc105 -layout usde -variant bouni
```

To set this automatically, copy the `10-keyboard.conf` to `/etc/X11/xorg.conf.d/`

## Thanks

This is mainly the work of [Roman Gerber](https://github.com/rgeber/xkb-layout-us-intl-de) with slight changes.

