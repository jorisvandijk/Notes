# Orphanded packages in Arch

Remove them by issuing this command:
```
sudo pacman -Rs $(pacman -Qqtd)
```