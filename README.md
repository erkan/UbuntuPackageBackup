# Ubuntu Package Backup and Restore
Most simple way to backup and reinstall all installed packages.

#### Create a Nightly Job:

``dpkg --get-selections > /home/username/installed-packages.list``

#### After a clean install, restore your home directory, set up your Non-Ubuntu repositories. Then to reinstall all:

``sudo apt update``

``sudo dpkg --set-selections < /home/username/installed-packages.list``

``sudo apt-get dselect-upgrade``

##### That's all
