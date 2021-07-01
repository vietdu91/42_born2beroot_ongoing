## **Born2BeRoot**  || **D2** | 🔥 Autoriser les connexions entrantes

__But :__ Autoriser les connexions SSH (comme avec le port 4242) avec UFW 

> Si tu actives ton pare-feu UFW, il refusera toutes les connexions entrantes. Cela signifie que tu devras créer des règles qui autorisent explicitement les connexions entrantes légitimes – connexions SSH ou HTTP, par exemple – si tu veux que ton serveur réponde à ce type de demandes.

*1. Pour autoriser les connections SSH entrantes, tu peux utiliser la commande* ```allow ssh``` :

```
vietdu91@bg42:~$ sudo ufw allow ssh
```

> UFW sait quel port ```allow ssh``` désigne parce qu'il est listé comme un service dans le fichier ```/etc/services```.

*2. Pour autoriser la connexion avec un port SSH spécifique, comme par exemple le port* ```4242```, *tu peux utiliser la commande* ```allow ssh``` :
```
vietdu91@bg42:~$ sudo ufw allow 4242
```

*3. Pour vérifier le statut de l'UFW, utilise la commande* ```ufw status``` :
```
vietdu91@bg42:~$ sudo ufw status
Status: active

To                         Action      From
--                         ------      ----
4242                       ALLOW       Anywhere
4242 (v6)                  ALLOW       Anywhere (v6)
```

