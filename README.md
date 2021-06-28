## SOMMAIRE || Born2BeRoot 42 - THE Project 

# :pencil2: *Système*

```A1.``` Modifier le hostname du système

```A2.``` Personnaliser le message d'accueil lors d'une connexion Shell

```A3.``` Afficher la liste et les caractéristiques des disques et des partitions (lsblk)


# :crown: *Administrateur et sudo*

```B1.``` Installer sudo (sudo . apt-get . dpkg -l)

```B2.``` Configurer /etc/sudoers (visudo)

```B3.``` Afficher des astérisques lors de la saisie du mot de passe (env_reset . pwfeedback)

```B4.``` Augmenter ou réduire le temps de grâce avant que la saisie du mot de passe soit de nouveau demandée (env_reset . timestamp_timeout)

```B5.``` Changer le message d'erreur de mauvais mot de passe (env_reset . badpass_message)

```B6.``` Modifier le nombre de tentatives de saisie de mot de passe autorisées (passwd_tries)

```B7.``` Créer un sudo Log File (logfile . log_host . log_year)

```B8.``` Créer une entrée/sortie de la commande sudo (log_input . log_output)

```B9.``` Définir un PATH sécurisé (secure_path)

```B10.``` Activer sudo sur la session de connexion de l'utilisateur TTY (requieretty)


# :key: *SSH*

```C1.``` Installer SSH (apt-get . openssh-server . dpkg - l)

```C2.``` Modifier un port SSH (sshd_config) 

```C3.``` Autoriser/Refuser l’accès root via SSH (PermitRootLogin)

```C4.``` Se connecter au serveur via SSH (ssh)


# :fire: *UFW*

```D1.``` Installer et démarrer UFW (apt-get . dpkg -l . enable)

```D2.``` Autoriser les connexions entrantes (allow)


# :speak_no_evil: *Gestion des mots de passe*

```E1.``` Modifier le mot de passe d'un utilisateur

```E2.``` Modifier la durée de vie d'un mot de passe (login.defs)

```E3.``` Etablir une politique de mot de passe fort (libpam-pwquality . common-password)


# 👥 *Groupes et utilisateurs*

```F1.``` Créer un nouvel utilisateur et l'attribuer à un groupe (useradd)

```F2.``` Ajouter un compte d'utilisateur existant à un groupe (usermod)

```F3.``` Changer le groupe principal d'un utilisateur (usermod)

```F4.``` Afficher les groupes auxquels un compte d'utilisateur est affecté (groups . id)

```F5.``` Vérifier si l'utilisateur est bien dans un groupe (getent)

```F6.``` Ajouter un nouveau groupe (groupadd)


# :scroll: *Scripts et Cron*

```G1.``` Petits rappels de commandes Shell ($ . cat . grep . echo . wc)

```G2.``` Créer un fichier .sh

```G3.``` Maîtriser l'art de la syntaxe de awk (awk)

```G4.``` Utiliser les conditions dans les scripts .sh (if . then . else . fi)

```G5.``` Utiliser les comparateurs dans les scripts .sh (-eq . -ne . -gt . -ge . -lt . -le . -z)

```G6.``` Editer le fichier de crontab (crontab)

```G7.``` Démarrer / Arrêter le processus de cron (start . stop) 


# 🗞 *Wordpress*

```H1.``` Installer Wordpress en local
