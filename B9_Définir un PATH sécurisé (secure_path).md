## **Born2BeRoot**  || **B9** | :crown: Définir un PATH sécurisé

__But :__ Sécuriser le PATH utilisé pour chaque commande exécutée avec ```sudo```

> Le PATH est une variable d'environnement qui liste les répertoires dans lesquels peuvent être placés des fichiers exécutables. Si un exécutable n'est pas placé dans l'un de ces répertoires, il sera nécessaire d'indiquer le chemin exact chaque fois qu'on l'appellera.

> Ce PATH sécurisé est utilisé lorsqu'un administrateur système ne fait pas confiance aux utilisateurs de ```sudo``` pour avoir une variable d'environnement PATH sécurisée. 

> Pour séparer ```root path``` et ```user path```, seuls les utilisateurs définis par ```exempt_group``` ne sont pas affectés par ce paramètre.


*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```secure_path="<chemin>"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin"
```
