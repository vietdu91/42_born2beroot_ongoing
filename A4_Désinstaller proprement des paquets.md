## **Born2BeRoot**  || **A4** | :pencil2: Désinstaller proprement des paquets

__But :__ Faire en sorte qu'il ne reste plus un seul octet d'un paquet indésirable dans la mémoire du système


> ⚠️ Faire attention : Vouloir supprimer trop de paquets peut conduire à l'instabilité du système, voire à ne plus pouvoir le redémarrer !

*1. Pour une suppression partielle d'un logiciel, utilise la commande* ```apt-get remove```, *suivi du paquet à supprimer :*
```
vietdu91@bg42:~$ sudo apt-get remove <paquet-a-supprimer>
```

*2. Pour supprimer les fichiers de configuration du paquet installé, qui ont été conservés par défaut, utilise la commande* ```apt-get remove --purge```, ou bien plus simplement ```apt-get purge```, *suivi du paquet à supprimer :*
```
vietdu91@bg42:~$ sudo apt-get purge <paquet-a-supprimer>
```

*3. Pour supprimer un logiciel et ses dépendances (du moins, celles qui ne sont pas utilisées par d'autres logiciels), utilise la commande* ```apt-get --purge autoremove```, *suivi du paquet à supprimer :*
```
vietdu91@bg42:~$ sudo apt-get --purge autoremove <paquet-a-supprimer>
```

> Il existe aussi plusieurs outils qui suppriment de manière plus simple les paquets indésirés, comme ```debfoster```, ```aptsh``` et j'en passe. Pour plus de détails : https://linuxfr.org/wiki/desinstaller-proprement-ses-paquets-sur-sa-distribution
