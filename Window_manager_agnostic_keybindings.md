#Window manager agnostic keybindings!

~/.xbindkeysrc:

```
"firefox"
  m:0x40 + c:25
  Mod4 + w
```

```
"firefox --private-window"
  m:0x40 + c:26
  Mod4 + e
```

Bindings begin to work as soon as you run xbindkeys command. If you want to have it on system start-up, add it to ~/.xinitrc (btw it means that those key bindings will work in login manager too!).

But how you figure out those m:0xNN +c:XX codes? Just run xbindkeys -k command in the terminal. It will spawn window. After you press your key combination, it will exit and print required codes.