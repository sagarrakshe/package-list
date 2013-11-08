The purpose of this repo is, to preserve the installed packages/appliations when migrating from my machine to other Ubuntu machine.

Export the current package list from your machine:

    sudo dpkg --get-selections > my_packages.txt

Select this list as the packages to install on new machine.

    sudo dpkg --set-selections < my_packages.txt
    sudo apt-get dselect-upgrade

