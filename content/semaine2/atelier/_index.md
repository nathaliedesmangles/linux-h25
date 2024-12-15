 
+++
title = "ATELIER: Les commandes Linux de base"
weight = 24
+++

## Objectif de l'atelier

Cet atelier a pour but de vous familiariser avec les commandes simples et de base sous Linux en utilisant Ubuntu comme distribution Linux. 
Les exercices pratiques permettront de renforcer la compréhension et l'utilisation de ces commandes.

{{% notice style=warning title=Attention %}}
Votre Windows 10/11 de votre VM doit être à jour.
{{% /notice %}}

## Préalables

### Mettre à jour Windows

**Pour Windows 10**:

Cliquer sur [Mise à jour de Windows 10](https://www.microsoft.com/fr-ca/software-download/windows10) et cliquer sur **Mettre à jour maintenant.**

**Pour Windows 11**:

Cliquer sur [Installer Windows Mise à jour](https://support.microsoft.com/fr-fr/windows/mettez-%C3%A0-jour-windows-3c5ae7fc-9fb6-9af1-1984-b5e0412c556a#WindowsVersion=Windows_11), puis cliquer sur **Rechercher les mises à jour de Windows** et suivre les étapes.

## Format de la remise

{{% notice style=warning title=Attention %}}
Pour chacune des étapes et questions vous devrez prendre une **capture d'écran de vos commandes et résultats**. **ATTENTION**: On doit pouvoir voir votre non d'utilisateur. Ne travaillez donc **pas** avec l'utilisateur `root`.
{{% /notice %}}

# Atelier

## Exercice #1: Navigation dans la structure de fichiers de Linux (Ubuntu)

### Partie 1: Installation et activation de WSL (*Windows Subsystem for Linux*)

1. Rechercher les fonctionnalités Windows

![Recherche fonctionnalités](recherche-fonctionnalites.png?width=25vw)

2. Dans la liste, cocher ***Sous-Système Windows pour Linux**

![Activer fonctionnalités](activer-fonctionnalite.png?width=25vw)

   - Prenez une capture d'écran de cette étape et nommez-la `1.png`.

3. Redémarrer

   - Prenez une capture d'écran de l'écran de redémarrage et nommez-la `2.png`.

Une fois redémarré, vous pouvez installer la distribution Ubuntu depuis le Microsoft Store.


### Partie 2: Installation d'Ubuntu

WSL prend en charge une variété de distributions Linux, y compris la dernière version LTS d'Ubuntu. 

Il existe plusieurs façons d'installer des distributions sur WSL, nous nous concentrons ici sur la méthode via l'application dans Microsoft Store et les commandes WSL exécutées dans le terminal. Le résultat est le même quelle que soit la méthode.

**Application dans Microsoft Store**

1. Ouvrir Microsoft Store et trouver la dernière version d'Ubuntu.

![Résultats de recherche pour Ubuntu 24.04 LTS dans la barre de recherche Windows.](search-ubuntu-windows.png?width=40vw)

2. Cliquez sur **Free/Gratuit**, puis sur **Get/Obtenir**.

![Page d'installation pour Ubuntu 24.04 LTS dans le Microsoft Store.](choose-distribution.png?width=40vw)

3. Patienter durant l’installation. Ubuntu sera alors installé sur votre machine. 

4. Avant de commencer, s’assurer qu’Ubuntu est à jour:
```plaintext
$ sudo apt update
```

**NOTE**: La commande `sudo` permet d’exécuter une commande en tant qu’administrateur du système.

Une fois installé, vous pouvez soit lancer l'application directement depuis le Microsoft Store, soit rechercher Ubuntu dans votre barre de recherche Windows.

- Prenez une capture d'écran de la fenêtre de terminal Ubuntu et nommez-la `3.png`.

---
**References**:  
1. [Site Ubuntu WSL](https://documentation.ubuntu.com/wsl/en/latest/guides/install-ubuntu-wsl2/)
2. [Vidéo YouTube](https://youtu.be/HrAsmXy1-78?si=VyvuNbkGmthsnLAI)
---


### Partie 3: Navigation dans la structure de fichiers

4. **Commande `date`**
   - Afficher la date et l'heure actuelles du système.**
   - Prenez une capture d'écran du résultat et nommez-la `4.png`.

5. **Commande `ls`**
   - Listez les fichiers et répertoires dans le répertoire courant en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `5.png`.

6. **Commande `pwd`**
   - Affichez le chemin du répertoire courant en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `6.png`.

7. **Commande `cd`**
   - Changez de répertoire pour le répertoire "home" en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `7.png`.

8. **Commande `ls -l`**
   - Listez les fichiers et répertoires avec des détails supplémentaires en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `8.png`.


## Exercice #2: Création, suppression et déplacement de fichiers et répertoires

{{% notice style=warning title=Attention %}}
Avant de commencer, assurez vous d'être dans votre répertoire personnel.
{{% /notice %}}


9. **Commande `mkdir`**
   - Créez deux nouveaux répertoires nommés "atelier2" et "atelier3" en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `9.png`.

10. **Commande `rmdir`**
   - Supprimez le répertoire "atelier3" en utilisant la commande.
   - Prenez une capture d'écran du résultat et nommez-la `10.png`.

11. **Commande `cd`**
    - Changez de répertoire pour le répertoire "atelier" en utilisant la commande.
    - Prenez une capture d'écran du résultat et nommez-la `11.png`.

12. **Commande `touch`**
    - Créez un nouveau fichier nommé "fichier.txt" en utilisant la commande.
    - Prenez une capture d'écran du résultat et nommez-la `12.png`.

13. **Commande `echo`**
    - Ajoutez du texte au fichier "fichier.txt" en utilisant la commande.
    - Prenez une capture d'écran du résultat et nommez-la `13.png`.

14. **Commande `cat`**
    - Affichez le contenu du fichier "fichier.txt" en utilisant la commande.
    - Prenez une capture d'écran du résultat et nommez-la `14.png`.

15. **Commande `mv`**
    - Déplacez le fichier "fichier.txt" vers un nouveau répertoire nommé "documents" en utilisant la commande:
    - Prenez une capture d'écran du résultat et nommez-la `15.png`.

16. **Commande `rm`**
    - Supprimez le fichier "fichier.txt" en utilisant la commande.
    - Prenez une capture d'écran du résultat et nommez-la `16.png`.

{{% notice style=note %}}
**NB** : pour les questions **#17** à **#20**, utiliser le texte disponible [ici](fichier2.txt). 
Copiez collez le texte dans un fichier texte nommé "fichier2.txt".
{{% /notice %}}

17. **Commande `mv`**
     - Déplacez le fichier dans votre répertoir atelier2.
     - Prenez une capture d'écran du résultat et nommez-la `17.png`.

18. **Commande `less`**
     - Affichez le contenu d'un fichier page par page, jusqu'à la dernière page.
     - Prenez une capture d'écran du résultat et nommez-la `18.png`.

19. **Commande `head`.**
     - Affichez les premières lignes du fichier.
     - Prenez une capture d'écran du résultat et nommez-la `19.png`.

20. **Commande `tail`.**
     - Affichez les dernières lignes du fichier.
     - Prenez une capture d'écran du résultat et nommez-la `20.png`.

21. **Commande `history`**
    - Affichez l'historique des commandes précédemment exécutées en utilisant la commande
    - Prenez une capture d'écran du résultat et nommez-la `21.png`.