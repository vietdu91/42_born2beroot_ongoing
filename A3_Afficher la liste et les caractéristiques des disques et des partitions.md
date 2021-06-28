## **Born2BeRoot**  || **A3** | :pencil2: Afficher la liste et les caractéristiques des disques et des partitions

__But :__ Lister les disques et les partitions du système

*1. Si l'utilitaire n'est pas présent dans ton système, installe-le : *
```
root@bg42:~$ apt-get update
root@bg42:~$ apt-get install util-linux
```

*2. Pour afficher les disques et les partitions du système, utilise la commande* ```lsblk``` :
```
vietdu91@bg42:~$ lsblk
NAME                    MAJ:MIN RM  SIZE RO TYPE  MOUNTPOINT
sda                       8:0    0    8G  0 disk
|-sda1                    8:1    0  132M  0 part  /boot
|-sda2                    8:2    0    1K  0 part
`-sda5                    8:5    0  7.9G  0 part
  `-sda5_crypt          254:0    0  7.9G  0 crypt
    |-LVMGroup-root     254:1    0  2.6G  0 lvm   /
    |-LVMGroup-swap     254:2    0  612M  0 lvm   [SWAP]
    |-LVMGroup-home     254:3    0  1.3G  0 lvm   /home
    |-LVMGroup-var      254:4    0  796M  0 lvm   /var
    |-LVMGroup-srv      254:5    0  796M  0 lvm   /srv
    |-LVMGroup-tmp      254:6    0  796M  0 lvm   /tmp
    `-LVMGroup-var--log 254:7    0    1G  0 lvm   /var/log
sr0                      11:0    1 1024M  0 rom
```

*3. Pour afficher les disques et les partitions du système avec certaines de leurs caractéristiques, utilise plutôt la commande* ```lsblk --output``` :
```
vietdu91@bg42:~$ lsblk -output NAME,SIZE,MOUNTPOINT
NAME                     SIZE MOUNTPOINT
sda                        8G
|-sda1                   132M /boot
|-sda2                     1K
`-sda5                   7.9G
  `-sda5_crypt           7.9G
    |-LVMGroup-root      2.6G /
    |-LVMGroup-swap      612M [SWAP]
    |-LVMGroup-home      1.3G /home
    |-LVMGroup-var       796M /var
    |-LVMGroup-srv       796M /srv
    |-LVMGroup-tmp       796M /tmp
    `-LVMGroup-var--log    1G /var/log
sr0                     1024M
```

> Pour plus de détails sur la commande ```lsblk```, je te conseille de lire le ```man lsblk``` !
