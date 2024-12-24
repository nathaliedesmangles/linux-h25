+++
title = "Structure du système de fichiers Linux"
weight = 22
+++

![Arborescence](filesystem.png?width=100vw)

La structure du système de fichiers Linux est hiérarchique et organisée sous la forme d'un arbre inversé, où la racine (root) est représentée par `/`. 
Tous les fichiers et répertoires sont situés sous cette racine. Comprendre cette structure est essentiel pour naviguer et gérer efficacement un système Linux.

La structure du système de fichiers Linux est conçue pour être logique et organisée, facilitant ainsi la gestion et la navigation. Chaque répertoire a un rôle spécifique et contient des types de fichiers bien définis. Comprendre cette structure est crucial pour tout utilisateur ou administrateur de système Linux.

## Répertoires principaux

1. **/** (Racine)
   - Le point de départ de l'arborescence du système de fichiers. Tous les autres répertoires et fichiers sont situés sous ce répertoire.

2. **/bin**
   - Contient les binaires essentiels nécessaires au démarrage du système et à l'exécution des commandes de base, comme `ls`, `cp`, `mv`, etc.

3. **/boot**
   - Contient les fichiers nécessaires au démarrage du système, y compris le noyau Linux et les fichiers de configuration du chargeur de démarrage (bootloader).

4. **/dev**
   - Contient les fichiers de périphériques. Chaque périphérique matériel (comme les disques durs, les clés USB, etc.) est représenté par un fichier dans ce répertoire.

5. **/etc**
   - Contient les fichiers de configuration du système. Par exemple, les fichiers de configuration des services, des utilisateurs, des réseaux, etc.

6. **/home**
   - Contient les répertoires personnels des utilisateurs. Chaque utilisateur a son propre répertoire sous `/home`, par exemple `/home/utilisateur`.

7. **/lib**
   - Contient les bibliothèques partagées nécessaires pour les binaires situés dans `/bin` et `/sbin`.

8. **/media**
   - Point de montage pour les périphériques amovibles comme les CD-ROM, les clés USB, etc.

9. **/mnt**
   - Utilisé pour monter temporairement des systèmes de fichiers. Par exemple, pour monter un disque dur externe.

10. **/opt**
    - Contient les logiciels optionnels et les paquets additionnels qui ne sont pas inclus dans la distribution standard.

11. **/proc**
    - Système de fichiers virtuel qui contient des informations sur les processus en cours et le système. Par exemple, `/proc/cpuinfo` contient des informations sur le processeur.

12. **/root**
    - Répertoire personnel de l'utilisateur root (administrateur du système).

13. **/run**
    - Contient des informations sur l'état du système depuis le dernier démarrage. Utilisé pour stocker des fichiers temporaires nécessaires au fonctionnement du système.

14. **/sbin**
    - Contient les binaires essentiels pour l'administration du système, comme `fdisk`, `ifconfig`, etc.

15. **/srv**
    - Contient les données spécifiques aux services fournis par le système. Par exemple, les fichiers de données pour un serveur web peuvent être stockés ici.

16. **/tmp**
    - Contient les fichiers temporaires créés par les utilisateurs et les applications. Ce répertoire est souvent vidé au redémarrage du système.

17. **/usr**
    - Contient les applications et les fichiers utilisés par les utilisateurs. Sous-répertoires importants :
      - **/usr/bin** : Contient les binaires des applications utilisateur.
      - **/usr/lib** : Contient les bibliothèques partagées pour les applications utilisateur.
      - **/usr/local** : Contient les logiciels installés localement par l'administrateur du système.

18. **/var**
    - Contient les fichiers variables, tels que les journaux système, les fichiers de spool, et les fichiers temporaires des applications. Par exemple, `/var/log` contient les fichiers journaux.
