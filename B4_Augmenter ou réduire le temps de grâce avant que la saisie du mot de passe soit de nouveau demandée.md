## **Born2BeRoot**  || **B4** | :crown: Augmenter ou réduire le temps de grâce avant que la saisie du mot de passe soit de nouveau demandée

__But :__ Faire en sorte qu'une valeur X doit être remplacée par la durée, en minutes, durant laquelle le mot de passe n'a pas à être fourni pour effectuer des actions d'administration dans le terminal. 

*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```timestamp_timeout=X``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      timestamp_timeout=X
```

> La valeur 0 désactive ce temps de grâce : un mot de passe doit être fourni à chaque action d'administration.
> Si cette option n'est pas précisée, le temps de grâce par défaut est 15 minutes.
