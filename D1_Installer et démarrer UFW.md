## **Born2BeRoot**  || **D1** | 🔥 Installer et démarrer UFW

__But :__ Installer et démarrer un pare-feu UFW dans un système d'exploitation

*1. Installe* UFW *via* ```apt-get``` *et cette ligne de commande* :

```
root@bg42:~$ apt-get install ufw
```

*2. Vérifie si* ```ufw``` *a été installé avec succès*

```
root@bg42:~$ dpkg -l | grep ufw
ii  ufw                            0.36-1                       all          program for managing a Netfilter firewall
root@bg42:~$
```

...

> ...
