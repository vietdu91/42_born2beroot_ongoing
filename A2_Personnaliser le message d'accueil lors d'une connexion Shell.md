## **Born2BeRoot**  || **A2** | :pencil2: Personnaliser le message d'accueil lors d'une connexion Shell

__But :__ Faire changer le message de bienvenue merdique de Debian pour un message d'accueil perso stylé

> ⚠️ Il faut avoir les privilèges root pour effectuer la personnalisation du message de bienvenue.

-- AVANT 🤮 :
```
The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the individual files in /usr/share/doc/*/copyright.

Devian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent permitted by applicable law.
```

-- AVANT 🤩 :
```
Bienvenue dans mon humble demeure BB.

    )                      (                                 )                     
 ( /(                      )\ )                       )   ( /(                     
 )\())         )      (   (()/( (  (      (    (   ( /(   )\())         )      (   
((_)\   (     (      ))\   /(_)))\))(    ))\  ))\  )\()) ((_)\   (     (      ))\  
 _((_)  )\    )\  ' /((_) (_)) ((_)()\  /((_)/((_)(_))/   _((_)  )\    )\  ' /((_) 
| || | ((_) _((_)) (_))   / __|_(()((_)(_)) (_))  | |_   | || | ((_) _((_)) (_))   
| __ |/ _ \| '  \()/ -_)  \__ \\ V  V // -_)/ -_) |  _|  | __ |/ _ \| '  \()/ -_)  
|_||_|\___/|_|_|_| \___|  |___/ \_/\_/ \___|\___|  \__|  |_||_|\___/|_|_|_| \___|  
```

*1. Edite le fichier* ```/etc/motd``` :
```
vietdu91@kassos42:~$ nano /etc/motd
```

*2. A travers l'éditeur, ajouter le contenu souhaité*

> Si tu veux pimper du texte en ASCII, tu peux le faire à travers le site patorjk.com

*3. Redémarre ton serveur et admire la beauté de ton message de bienvenue*
