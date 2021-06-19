##SOMMAIRE || Born2BeRoot - THE Project 
==========================================================================

#:pencil2: *Système*

**A1.** Modifier le hostname du système


#:crown: *Administrateur et sudo*

**B1.** Installer sudo (sudo . apt-get . dpkg -l)

**B2.** Configurer /etc/sudoers (visudo)

**B3.** Afficher des astérisques lors de la saisie du mot de passe (env_reset . pwfeedback)

**B4.** Augmenter ou réduire le temps de grâce avant que la saisie du mot de passe soit de nouveau demandée (env_reset . timestamp_timeout)

**B5.** Changer le message d'erreur de mauvais mot de passe (env_reset . badpass_message)

**B6.** Modifier le nombre de tentatives de saisie de mot de passe autorisées (passwd_tries)

**B7.** Créer un sudo Log File (logfile . log_host . log_year)

**B8.** Créer une entrée/sortie de la commande sudo (log_input . log_output)

**B9.** Définir un PATH sécurisé (secure_path)

**B10.** Activer sudo sur la session de connexion de l'utilisateur TTY (requieretty)


#:key: *SSH*

**C1.** Installer SSH (apt-get . openssh-server . dpkg - l)

**C2.** Modifier un port SSH (sshd_config) 

**C3.** Autoriser/Refuser l’accès root via SSH (PermitRootLogin)


#:fire: *UFW*

**D1.** ...


#:speak_no_evil: *Gestion des mots de passe*

**E1.** Modifier le mot de passe d'un utilisateur


#:people_hugging: *Groupes et utilisateurs*

**F1.** Créer un nouvel utilisateur et l'attribuer à un groupe (useradd)

**F2.** Ajouter un compte d'utilisateur existant à un groupe (usermod)

**F3.** Changer le groupe principal d'un utilisateur (usermod)

**F4.** Afficher les groupes auxquels un compte d'utilisateur est affecté (groups . id)

**F5.** Vérifier si l'utilisateur est bien dans un groupe (getent)

**F6.** Ajouter un nouveau groupe (groupadd)


#:scroll: *Scripts et Cron*

**G1.** ...