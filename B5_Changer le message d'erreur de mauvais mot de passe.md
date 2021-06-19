## **Born2BeRoot**  || **B5** | :crown: Changer le message d'erreur de mauvais mot de passe

__But :__ Ajouter un message d'erreur personnalisé en cas de mot de passe incorrect :
```
vietdu91@bg42:~$ sudo apt_get update
[sudo] password for vietdu91 :
T'es bourré.e ou quoi ? C'est sérieux là, écris bien le MDP !
[sudo] password for vietdu91 :
```

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```badpass_message="<texte à afficher>"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      badpass_message="T'es bourré.e ou quoi ? C'est sérieux là, écris bien le MDP !"
```
