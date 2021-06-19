## **Born2BeRoot**  || **B1** | :crown: Installer sudo 

**But : **Installer sudo, absent dans un système d'exploitation

*1. Mets-toi en mode* root *via la commande* su
```vietdu91@bg42:~$ su
Password :
root@bg42:~$```
*2. Installe* sudo *via* apt-get *et cette ligne de commande* :
```root@bg42:~$ apt-get install sudo```
3. Vérifie si sudo a été installé avec succès 
```root@bg42:~$ dpkg -l | grep sudo
ii  sudo              1.8.27-1+deb10u3           amd64      Provide limited super user privileges to specific users
root@bg42:~$```
:bookmark:  La commande *dpkg -l* sert vérifier la présence d'un paquet. Les deux premiers caractères à gauche te donnent des indications sur l'état du paquet
Plus de détails : https://doc.ubuntu-fr.org/dpkg