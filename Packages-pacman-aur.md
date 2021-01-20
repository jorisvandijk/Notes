# Pacman / AUR packages listing

Create a list of packages installed
```
pacman -Qqe > pkglist.txt
```
Create a list of installed applications in AUR
```
    pacman -Qqm > pkglist_aur.txt
```

Running the following will highlight the AUR packages in the pacman list.
```
    sudo pacman -S - < pkglist.txt
```

