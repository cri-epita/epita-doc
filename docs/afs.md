# AFS (Andrew File System)

Since the start of the 2016 schoolyear, [AFS](https://www.openafs.org/)  replaces [GlusterFS](https://www.gluster.org) for network shares and student accounts.

## Linux session

## AFS folder

By logging in with login and password, an afs folder is automatically mounted at one's root folder : `/home/login/afs`. It is essential to understand that anything that is not located in this folder will be erased on reboot. Labors should be saved in this folder.

## AFS configuration

At account creation, plenty of configuration files are set in the .confs folfer of afs : `/home/login/afs/.confs/`.

For configuration to be taken into account, the script `/home/login/afs/.confs/install.sh` is called on each session boot and deals with symbolic links in folders. For example : `ln -s $AFS_DIR/.confs/bashrc $HOME/.bashrc`. It is possible to add new links in this file.

Those configuration files being symbolic links, it is identical to modify `/home/my_login/afs/.confs/bashrc` and `/home/my_login/.bashrc`. To see all links, one should type ls -la in his terminal, being in his personnal folder.

It is possible to retrieve initial configuration in the folder : `/afs/cri.epita.net/resources/confs/`.
