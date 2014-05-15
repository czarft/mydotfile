My Dot file 
=========

### Add Synapse PPA ###

The configuration uses an application launcher called Synapse. Synapse used to be in the Ubuntu repositories as of 12.04 but is no longer there in 14.04. Apparently it was not updated to work with the appropriate versions of the libraries it uses in time for the release. Therefore, in order to keep synapse working, the install script adds a PPA with development builds of Synapse. If this situation changes I will update the installer to use a more stable source for this package. 

If you want to add this PPA manually, run this command:

    sudo apt-add-repository ppa:synapse-core/testing
    sudo apt-get update

### Install packages ###

This xmonad configuration uses a variety of different packages. Some of them are required for xmonad, others are not specific to xmonad but are core parts of the overall desktop configuration, and others are simply tools which I use frequently enough that my default configuration runs them on startup.

If you want to install the entire list of packages, you can run the following command:

    sudo apt-get install xmonad libghc-xmonad-dev libghc-xmonad-contrib-dev xmobar xcompmgr nitrogen stalonetray moreutils synapse consolekit ssh-askpass-gnome thunar terminator remmina

If you prefer to pick and choose, the following packages can be omitted while still maintaining the overall functionality:
 * remmina
 * thunar
 * ssh-askpass-gnome

