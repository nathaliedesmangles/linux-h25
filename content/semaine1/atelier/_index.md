+++
title = "ATELIER #1: Installation de Linux sur une VM"
weight = 14
alwaysopen = true
+++

## A FAIRE

- Simplifier, mettre juste les grandes idées et objectifs
- Lien vers page de l'atelier

## Objectifs

L'atelier a pour but de vous guider à travers le processus d'installation de Linux sur une machine virtuelle (VM). Cela permet d'expérimenter avec Linux sans affecter le système d'exploitation principal de l'ordinateur.

## Prérequis pour l’installation

1. Vous devez avoir téléchargé et installé un logiciel de virtualisation tel que VMWare Workstation Pro.
	- [Guide d'installation de VMware](À VENIR)
2. Vous devez avoir téléchargé la dernière version d'Alma Linux.
	- [Alma Linux](https://almalinux.org/get-almalinux/)
	- Choisissez une miroir et téléchargez ***AlmaLinux-9.5-x86_64-dvd.iso***.
	
	![Image ISO Alma Linux](telecharger-alma.png)

- VMWare permet d’installer différents systèmes d’exploitation sur une même machine.
- Le nombre de machines virtuelles que l’on peut installer dépend de la puissance en terme de CPU et de mémoire de la machine hôte.
- La machine hôte est celle qui héberge les machines virtuelles.
- La machine hôte peut être Windows ou Linux et les invités peuvent être une grande variété de systèmes d’exploitation.

## Installation d'Alma Linux

[Guide d'installation d'Alma Linux](.pdf)
https://wiki.almalinux.org/documentation/installation-guide.html#requirements




---

3. **Création d'une nouvelle machine virtuelle**
   - Ouvrez VMware.
   - Cliquez sur "Nouvelle" pour créer une nouvelle machine virtuelle.
   - Donnez un nom à votre VM (par exemple, "Linux VM") et sélectionnez le type et la version du système d'exploitation (par exemple, Linux et Ubuntu 64-bit).
   - Allouez de la mémoire RAM à la VM (au moins 2 Go recommandés).
   - Créez un disque dur virtuel en suivant les instructions (taille recommandée : au moins 20 Go).

4. **Configuration de la machine virtuelle**
   - Sélectionnez la VM nouvellement créée et cliquez sur "Paramètres".
   - Allez dans l'onglet "Stockage" et ajoutez un lecteur optique virtuel.
   - Sélectionnez l'image ISO de Linux que vous avez téléchargée précédemment.

5. **Démarrage de la machine virtuelle**
   - Sélectionnez la VM et cliquez sur "Démarrer".
   - La VM démarrera à partir de l'image ISO et vous verrez l'écran d'installation de Linux.

6. **Installation de Linux**
   - Suivez les instructions à l'écran pour installer Linux. Cela inclut la sélection de la langue, la configuration du réseau, le partitionnement du disque, et la création d'un compte utilisateur.
   - Une fois l'installation terminée, redémarrez la VM.

7. **Post-Installation**
   - Après le redémarrage, retirez l'image ISO du lecteur optique virtuel pour éviter de redémarrer sur l'installateur.
   - Connectez vous avec le compte utilisateur que vous avez créé.
   - Mettez à jour le système et installez les logiciels nécessaires via le gestionnaire de paquets de la distribution (par exemple, `apt` pour Ubuntu).


Vous avez maintenant une machine virtuelle Linux fonctionnelle. Vous pouvez utiliser cette VM pour explorer Linux, installer des logiciels, et pratiquer des commandes sans risquer de perturber votre système principal.

