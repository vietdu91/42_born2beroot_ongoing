## **Born2BeRoot**  || **B3** | :crown: Afficher des astérisques lors de la saisie du mot de passe

__But :__ Faire en sorte qu'il y ait des astérisques lors de la saisie du mot de passe, comme dans ce cas :
```
vietdu91@bg42:~$ sudo apt_get update
[sudo] password for vietdu91 : ************
```

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```pwfeedback``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      pwfeedback
```
