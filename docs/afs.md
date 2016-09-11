# AFS (Andrew File System)

Depuis la rentrée 2016, l'[AFS](https://www.openafs.org/) remplace
[GlusterFS](https://www.gluster.org) pour les partages réseaux et les comptes
des étudiants.

## Session Linux

### Dossier afs

En se connectant avec son login et son mot de passe, un dossier afs est
automatiquement monté à la racine de son dossier personnel:
`/home/my_login/afs`. Il est important de comprendre que tout ce qui n'est pas
dans ce dossier sera effacé au redémarrage de la machine. Il faut donc
sauvegarder son travail dans ce dossier.

### Gestion de sa configuration

Lors de la création du compte, un certain nombre de fichiers de configuration
ont été mis dans le dossier .confs du dossier afs : `/home/my_login/afs/.confs`.

Pour que les configurations soient prises en compte, le script
`/home/my_login/afs/.confs/install.sh` est appelé à chaque démarrage de session
et s'occupe de faire les liens symboliques dans son dossier personnel. Par
exemple : `ln -s $AFS_DIR/.confs/bashrc $HOME/.bashrc`. Il est possible
d'ajouter de nouveaux liens dans ce fichier.

Ces fichiers de configuration étant des liens symboliques, il est identique de
modifier `/home/my_login/afs/.confs/bashrc` et `/home/my_login/.bashrc`. Pour
voir la totalité des liens, il faut taper la commande `ls -la` dans son
terminal, en étant dans son dossier personnel.

Il est possible de récupérer les configurations initiales dans le dossier :
`/afs/cri.epita.net/resources/confs/`.
