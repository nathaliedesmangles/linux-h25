+++
title = "Guide d'installation d'AlmaLinux sur VMWare Workstation"
weight = 17
+++

## Prérequis
- **VMWare Workstation 17 Pro** installé sur votre machine.
- **ISO d'AlmaLinux 9.5** que vous pouvez télécharger depuis le site officiel d'AlmaLinux.
- **Connexion Internet** pour télécharger les fichiers nécessaires.

## Étapes d'installation

1. **Télécharger l'ISO d'AlmaLinux 9.5**:
   - Rendez-vous sur le [site officiel d'AlmaLinux](https://almalinux.org/get-almalinux/) et téléchargez l'ISO correspondant à AlmaLinux 9.5.
   - Le fichier téléchargé devrait se nommer  ***AlmaLinux-9.5-x86_64-dvd.iso***. (si la version actuelle est 9.5)
	
   ![Image ISO Alma Linux](../telecharger-alma.png)

2. **Créer une nouvelle machine virtuelle**:
   - Ouvrez VMWare Workstation Pro.
   - Cliquez sur ***"Create a New Virtual Machine"***.
   - Sélectionnez ***"Typical (recommended)"*** et cliquez sur ***"Next"***.
   - Choisissez **"Installer disc image file (iso)"** et parcourez pour sélectionner l'ISO d'AlmaLinux que vous avez téléchargé.
   - Cliquez sur **"Next"**.

3. **Configurer la machine virtuelle**:
   - Sélectionnez **"Linux"** comme système d'exploitation invité et ***"Red Hat Enterprise Linux 8 64-bit"*** comme version.
   - Donnez un nom à votre machine virtuelle (ex. Linux) et choisissez l'emplacement où vous souhaitez la stocker.
   - Allouez **au moins 20 Go** d'espace disque (recommandé).
   - Configurez la **mémoire RAM** à **au moins 2 Go** (recommandé).

4. **Personnaliser le matériel**:
   - Cliquez sur ***"Customize Hardware"***.
   - Ajustez les paramètres de processeur, de mémoire, de réseau, etc., selon vos besoins.
   - Assurez-vous que le lecteur de CD/DVD est configuré pour utiliser l'ISO d'AlmaLinux 9.5.
   - Cliquez sur ***"Close"*** puis sur ***"Finish"***.

5. **Démarrer la machine virtuelle**:
   - Sélectionnez votre nouvelle machine virtuelle et cliquez sur ***"Power on this virtual machine"***.
   - L'installation d'AlmaLinux 9.5 commencera automatiquement.

6. **Installation d'AlmaLinux 9.5**:
   - Suivez les instructions à l'écran pour installer AlmaLinux.
   - Sélectionnez la langue et le clavier.
   - Configurez le réseau et le nom d'hôte.
   - Choisissez le disque d'installation et configurez les partitions si nécessaire.
   - Sélectionnez les logiciels à installer.
   - Configurez le mot de passe root et créez un utilisateur.

7. **Finaliser l'installation**:
   - Cliquez sur "Begin Installation".
   - Attendez que l'installation se termine.
   - Une fois l'installation terminée, cliquez sur "Reboot" pour redémarrer la machine virtuelle.

8. **Post-installation**:
   - Après le redémarrage, connectez-vous avec les informations d'identification que vous avez créées.
   - Mettez à jour le système en utilisant la commande `dnf update`.

Vous avez maintenant AlmaLinux 9.5 installé sur une machine virtuelle VMWare Workstation 17.6.1 Pro. 