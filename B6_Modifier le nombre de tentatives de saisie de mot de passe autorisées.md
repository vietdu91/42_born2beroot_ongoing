## **Born2BeRoot**  || **B6** | :crown: Modifier le nombre de tentatives de saisie de mot de passe autorisées

__But :__ Limiter l'authentification à l'aide de sudo à X tentatives en cas de mot de passe incorrect :
```
vietdu91@bg42:~$ sudo apt_get update
[sudo] password for vietdu91 :
Password is wrong, please try again
[sudo] password for vietdu91 :
Password is wrong, please try again
[sudo] password for vietdu91 :
Password is wrong, please try again
sudo : 3 incorrect password attemps
vietdu91@bg42:~$
```

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```passwd_tries=X``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      passwd_tries=X
```

>  La valeur de limite par défaut est de 3.
