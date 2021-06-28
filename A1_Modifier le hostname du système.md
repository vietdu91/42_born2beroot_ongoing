## **Born2BeRoot**  || **A1** | :pencil2: Modifier le hostname du système

__But :__ Modifier le nom actuel du hostname ```kassos42``` en ```bg42```

*1. Vérifie bien le nom du hostname sur le terminal*
```
vietdu91@kassos42:~$ hostname
kassos42
```

*2. Cherche dans* ```/etc``` *le fichier* ```hostname``` *et le modifier avec le nom souhaité*

-- AVANT :
```
vietdu91@kassos42:~$ cd /etc
vietdu91@kassos42:~$ cat hostname
kassos42
```
-- APRES :
```
vietdu91@kassos42:~$ cat hostname
bg42
```

*3. Change le nom d'hôte dans un fichier d'hôtes : éditer* ```/etc/hosts```, *recherche le nom d'hôte actuel dans* ```127.0.0.1``` *et la ligne des adresses IP du serveur (le cas échéant) et la mettre à jour avec celle que tu as configurée ci-dessus

-- AVANT :
```
vietdu91@kassos42:~$ cat /etc/hosts
127.0.0.1    localhost
127.0.1.1    kassos42
```
-- APRES :
```
vietdu91@kassos42:~$ cat /etc/hosts
127.0.0.1    localhost
127.0.1.1    bg42
```

*4. Exécute le* ```hostname``` *commande avec la valeur souhaitée*
```
vietdu91@kassos42:~$ hostname bg42
```

*5. Reconnecte ton serveur et tu remarqueras ton nouveau nom d'hôte*
