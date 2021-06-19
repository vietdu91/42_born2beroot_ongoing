## **Born2BeRoot**  || **F4** | 👥  Afficher les groupes auxquels un compte d'utilisateur est affecté

__But :__ Afficher les groupes auxquels le compte d'utilisateur actuel est affecté et afficher les identifiants numériques associés à chaque groupe

*1. Pour afficher les groupes auxquels le compte d'utilisateur actuel est affecté , exécute la commande* ```groups```. *Tu verras une liste de groupes*
```
vietdu91@bg42:~$ groups
vietdu91 sudo user42
```
*2. Pour afficher les identifiants numériques associés à chaque groupe, exécutez plutôt la commande* ```id```
```
vietdu91@bg42:~$ id
uid=1000(vietdu91) gid=1000(vietdu91) groups=1000(vietdu91),27(sudo),1001(user42)
```
*3. Pour afficher les groupes d'un compte d'utilisateur spécifique, exécute la commande* ```groups``` *et spécifie le nom du compte utilisateur*
```
vietdu91@bg42:~$ groups marceldu56
marceldu56 sudo user42
```
*4. Pareil pour* ```id```
```
vietdu91@bg42:~$ id marceldu56
uid=1000(marceldu56) gid=1000(marceldu56) groups=1000(marceldu56),27(sudo),1001(user42)
```

> Le premier groupe de la liste *groups* ou le groupe affiché après ```gid =``` dans la liste ```id``` est le groupe principal du compte d'utilisateur. Les autres groupes sont les groupes secondaires.
