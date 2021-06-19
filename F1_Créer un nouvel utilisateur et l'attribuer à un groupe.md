## **Born2BeRoot**  || **F1** | 👥  Créer un nouvel utilisateur et l'attribuer à un groupe 

__But :__ Spécifier les groupes (*sudo*) auxquels un compte d'utilisateur *marceldu56* sera affecté lors de la création du compte utilisateur

*1. Crée un nouvel utilisateur et assigne ce compte au groupe souhaité via la commande* useradd
```
vietdu91@bg42:~$ sudo useradd -G sudo marceldu56
```

*2. Attribue un mot de passe pour cet utilisateur*

```
vietdu91@bg42:~$ passwd marceldu56
```