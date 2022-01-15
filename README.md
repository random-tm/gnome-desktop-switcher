# gnome-desktop-switcher
A helper script to change the desktop files in ~/.local/share/applications. This is typically used by desktops like gnome to show the applications you have available.

## How it works
It works by removing all desktop apps currently in the folder and then creating symbolic links back to two folders named all and one provided by the user when the script is run.

To reiterate this script assumes that your ~/.local/share/applications is something you intend to keep empty and just use symbolic links. It will erase all desktop files in the folder when run. This is not a bug. To use the script you need to remove the exit line; this is done to stop people from running the file blindly and wiping out a folder.

## How to use
Just create two folders with the paths. /mnt/custom-software/all and /mnt/custom-software/whatever-name-you-want-here. Then move the desktop files you want for all applications to all and the ones you want for your set of desktop files.