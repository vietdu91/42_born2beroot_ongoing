## **Born2BeRoot**  || **D1** | 🔥 Installer et démarrer UFW

__But :__ Installer et démarrer un pare-feu UFW dans un système d'exploitation

> Un pare-feu (ou _firewall_) est un système permettant de protéger un ordinateur ou un réseau d'ordinateurs des intrusions provenant d'un réseau tiers (comme Internet). Le pare-feu est donc un système permettant de filtrer les paquets de données échangés avec le réseau. 

> Le pare-feu UFW, ou Uncomplicated Firewall, est le pare-feu installé par défaut d'Ubuntu, un outil de configuration simplifié en ligne de commande sous GNU/Linux. Si tu souhaites commencer à sécuriser ton réseau, et tu n'es pas sûr de l'outil à utiliser, UFW peut être le bon choix pour toi.

*1. Installe* UFW *via* ```apt-get``` *et cette ligne de commande* :

```
vietdu91@bg42:~$ sudo apt-get install ufw
```

*2. Vérifie si* ```ufw``` *a été installé avec succès*

```
vietdu91@bg42:~$ dpkg -l | grep ufw
ii  ufw                            0.36-1                       all          program for managing a Netfilter firewall
vietdu91@bg42:~$
```

*3. Active le pare-feu UFW*
```
vietdu91@bg42:~$ sudo ufw enable
```
