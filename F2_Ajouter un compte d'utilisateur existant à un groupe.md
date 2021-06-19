## **Born2BeRoot**  || **F2** | 👥  Ajouter un compte d'utilisateur existant à un groupe

__But :__ Ajouter l'utilisateur *vietdu91* au groupe *sudo*

*1. Utilise le* ```usermod``` , *par le nom du groupe auquel tu veux ajouter l'utilisateur et avec le nom de l'utilisateur que tu veux ajouter*
```
vietdu91@bg42:~$ sudo usermod -a -G sudo vietdu91
```

> :warning: Sans le flag ```-a```,  l'instruction ajoute bien l’utilisateur au groupe mais en l’enlevant des groupes auxquels il appartient déjà ! Il faut donc tout simplement ajouter ```-a```, qui ajoute les nouveaux droits à l’utilisateur sans retirer les droits précédemment acquis. 
> **DE PLUS :** le paramètre ```-a``` doit impérativement se trouver avant ```-G``` car ```-G``` suppose que ```-a``` est un groupe.
