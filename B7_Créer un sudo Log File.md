## **Born2BeRoot**  || **B7** | :crown: Créer un sudo Log File

__But :__ Créer un fichier journal personnalisé de ```sudo``` à travers le paramètre ```logfile```
```
vietdu91@bg42:~$ cat /var/log/sudo.log
Jun 20 03:58:05 : root : TTY=pts/0 ; PWD=/ ; USER=root ; TSID=00000N ;
   COMMAND=/usr/bin/chage -1 emtran
Jun 20 04:22:30 : root : TTY=pts/0 ; PWD=/ ; USER=root ; TSID=00000O ;
   COMMAND=/usr/bin/nano /etc/sudoers.d
Jun 20 04:24:21 : root : TTY=pts/0 ; PWD=/etc/sudoers.d ; USER=root ;
   TSID=00000O ; COMMAND=/usr/sbin/visudo
vietdu91@bg42:~$
```

> Un *log file* (ou fichier journal) est un fichier de données généré par un ordinateur qui contient des informations sur les modèles d'utilisation, les activités et les opérations au sein d'un système d'exploitation, d'une application, d'un serveur ou d'un autre périphérique. 

> Par défaut, sudo enregistre les données via syslog(3). 

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```logfile="<chemin>"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      logfile="/var/log/sudo.log"
```
*2. Pour enregistrer le nom d'hôte et l'année à quatre chiffres dans le fichier journal personnalisé, utilisez les paramètres* ```log_host``` *et* ```log_year``` *respectivement comme suit :*
```
# See the man page for details on how to write a sudoers file.
#
Defaults      log_host, log_year, logfile="/var/log/sudo.log"
```
