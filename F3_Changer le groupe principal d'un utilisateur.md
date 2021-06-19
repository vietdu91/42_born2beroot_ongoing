## **Born2BeRoot**  || **F3** | 👥  Changer le groupe principal d'un utilisateur

__But :__ Assigner/Modifier l'utilisateur *vietdu91* dans le groupe *les_copains* en tant que groupe principal

> Alors qu'un compte d'utilisateur peut faire partie de plusieurs groupes, l'un des groupes est toujours le "groupe principal" et les autres sont des "groupes secondaires". Le processus de connexion de l'utilisateur et les fichiers et dossiers créés par l'utilisateur seront affectés au groupe principal.

*1. Exécute la commande* usermod, *avec le nom du groupe qui sera le groupe principal pour l'utilisateur, avec le nom du compte d'utilisateur*
```
vietdu91@bg42:~$ sudo usermod -g les_copains gaillard
```

> Lorsque tu utilises un flag *-g* en minuscule, tu affectes un groupe principal, alors que si tu utilises une majuscule *-G*, tu affectes un nouveau groupe secondaire (voir **F2**)
