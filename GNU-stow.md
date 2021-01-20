# GNU/Stow - an easy way to back up dotfiles!

For this example we're going to back up our i3 config file.

Install Stow (in Arch)
```
    sudo pacman -S stow
```
Prepare Stow directory
```
    cd ~ 
    mkdir Dotfiles
    cd Dotfiles
```
Next, to keep things organised, we'll create a directory for this and any future i3 files we want to stow.
```
    mkdir i3
    cd i3
```
This folder should be seen as a merely a title for what is to be put inside. It is not part of the file structure, as far as Stow is concerned.

Confusingly in order for Stow to work properly you will need to mirror the exact file structure as it currently is for the example file ~/.config/i3/config
you will need to *pretend* that the newly created ~/Dotfiles/i3 directory is the root of your home folder.

So the proper file structure (in this case) should be:

**~/Dotfiles/i3/.config/i3/config**

(~/STOW DIR/TITLE DIR/ACTUAL/FILESTRUCTURE/FILE)
```
    mkdir .config
    cd .config
```
Now you can copy the i3 dir from the actual ~/.config/i3/ to here (in this example I am assuming that only the config file is in that folder. If there are more, all of them will be stowed as well.)
```
    mv ~/.config/i3 ~/Dotfiles/i3/.config/
```
Now go into the ~/Dotfiles directory and run the Stow command to automagically create the symlinks for all files and directories added, needed to make this work.
```
    cd ~/Dotfiles
    stow -t ~ *
```
Instead of * you can also specify exactly what you want to stow.


The whole point of this is not having to mess with symlinks yourself, not needing to create a Bare repository and easilly backing up any dotfiles from all over your system from one single directory, with one normal .git repo. 

*Setting up the repo is out of the scope of this article.*

*The moving of folders and files can get a little hectic, and is also easilly done with a GUI file manager.*
