## **Born2BeRoot**  || **B10** | :crown: Activer sudo sur la session de connexion de l'utilisateur TTY

__But :__ Permettre à ```sudo``` d'être invoqué à partir d'un vrai tty


*1. Après être positionné dans* ```/etc/sudoers.d```,  *ajoute l'option* ```requiretty"``` *à la fin de la ligne débutant par* ```Defaults``` :
```
# See the man page for details on how to write a sudoers file.
#
Defaults      requeretty
```

> Le nom de TTY vient en fait à l'époque des ordinateurs : ils avaient des téléscripteurs comme terminaux, de sorte que tu pouvais voir la sortie des programmes imprimés (tty = TeleTYpe/TeleTYpewrite). TTY se réfère généralement aujourd'hui à des terminaux "physiques", comme plusieurs terminaux attachés (même comme un téléscripteur) à un seul ordinateur, ou de nos jours.

> Dans le cas d'Ubuntu, ```tty7``` est généralement utilisé par Xorg, qui fournit ton environnement graphique (pour être plus exact, il fournit un "système de fenêtrage" seulement, et des choses comme le gnome - comme une solution d'environnement de bureau - fonctionne "par-dessus").
> C'est également le cas si tu utilises ```ssh``` pour te connecter à une machine distante, donc en résumé : à chaque fois, quelque chose a besoin d'une fonctionnalité de type terminal/tty sans avoir un "vrai" tty.

> Plus de détails : https://azurplus.fr/quest-ce-quun-tty-sous-linux-et-comment-utiliser-la-commande-tty/
