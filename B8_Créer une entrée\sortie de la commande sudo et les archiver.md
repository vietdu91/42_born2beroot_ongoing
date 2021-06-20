## **Born2BeRoot**  || **B8** | :crown: Créer une entrée/sortie de la commande sudo et les archiver

__But :__ Créer une entrée/sortie de la commande sudo et les archiver
```
vietdu91@bg42:~$ cd /var/log/sudo
vietdu91@bg42:~$ ls
00  seq
vietdu91@bg42:~$ cd 00/00/01/
vietdu91@bg42:~$ ls
log stderr  stdin stdout  timing  ttyin ttyout
vietdu91@bg42:~$ cat log
1624027746:vietdu91:root::/dev/tty1:37:100
```

> Les paramètres ```log_input``` et ```log_output``` permettent à sudo d'exécuter une commande en pseudo-tty et de consigner toutes les entrées de l'utilisateur et toutes les sorties envoyées à l'écran de manière réceptive.

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```log_input, log_output"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      log_input, log_output
```

> Le répertoire par défaut du journal des entrées/sorties est ```/var/log/sudo-io```, et s'il existe un numéro de séquence de session, il est stocké dans ce répertoire. Tu peux spécifier un répertoire personnalisé via le paramètre ```iolog_dir```

*2. Pour archiver toutes les entrées et sorties sudo dans* ```/var/log/sudo/```, *ajoute l'option* ```log_input, log_output"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      log_input, log_output
Defaults      iolog_dir="/var/log/sudo"
```
