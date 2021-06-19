## **Born2BeRoot**  || **F5** | 👥  Vérifier si l'utilisateur est bien dans un groupe

__But :__ Vérifier si l'utilisateur a été ajouté avec succès au groupe *sudo*

*1. Tape cette ligne de commande* :
```
vietdu91@bg42:~$ getent group sudo
sudo:x:27:vietdu91
```
*2. Tu peux aussi taper cette ligne pour une meilleure visibilité* :
```
vietdu91@bg42:~$ getent group sudo | cut -d: -f4
vietdu91
```

> Le programme *getent* récupère des entrées dans la base de données d’administration spécifiée en utilisant la clé de recherche spécifiée.
Plus de détails : http://manpages.ubuntu.com/manpages/trusty/fr/man1/getent.1.html
