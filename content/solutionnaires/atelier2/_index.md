 
+++
title = "ATELIER02: Les commandes Linux de base (SOLUTION)"
weight = 152
+++

## Exercices pratiques

1. **Afficher la date et l'heure actuelles du système**
     ```bash
     date
     ```

2. **Changer le mot de passe de l'utilisateur**
     ```bash
     passwd
     ```

3. **Afficher le contenu d'un fichier.**
     - Créez un fichier texte avec du contenu :
        ```bash
        echo "Bonjour, Linux!" > fichier.txt
        ```
     - Tapez la commande suivante pour afficher le contenu du fichier et appuyez sur Entrée :
        ```bash
        cat fichier.txt
        ```
     - Observez la sortie qui affiche le contenu du fichier.

4. **Afficher le contenu d'un fichier page par page.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        less fichier.txt
        ```
     - Utilisez les touches suivantes pour naviguer :
        - `Espace` : Page suivante
        - `b` : Page précédente
        - `q` : Quitter

5. **Afficher les premières lignes d'un fichier.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        head fichier.txt
        ```
     - Pour afficher un nombre spécifique de lignes, utilisez l'option `-n` :
        ```bash
        head -n 5 fichier.txt
        ```

6. **Afficher les dernières lignes d'un fichier.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        tail fichier.txt
        ```
     - Pour afficher un nombre spécifique de lignes, utilisez l'option `-n` :
        ```bash
        tail -n 5 fichier.txt
        ```
     - Pour afficher les nouvelles lignes ajoutées en temps réel, utilisez l'option `-f` :
        ```bash
        tail -f fichier.txt
        ```

7. **Exécuter plusieurs commandes sur une seule ligne.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        date ; whoami
        ```
     - Observez la sortie qui affiche la date et l'heure suivies du nom de l'utilisateur actuel.

8. **Afficher le chemin complet du répertoire courant.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        pwd
        ```
     - Observez la sortie qui affiche le chemin complet du répertoire courant.

9. **Lister les fichiers et répertoires dans le répertoire courant.**
     - Tapez la commande suivante et appuyez sur Entrée :
        ```bash
        ls
        ```
     - Pour afficher les détails des fichiers et répertoires, utilisez l'option `-l` :
        ```bash
        ls -l
        ```
     - Pour afficher tous les fichiers, y compris les fichiers cachés, utilisez l'option `-a` :
        ```bash
        ls -a
        ```
     - Pour afficher les tailles de fichiers dans un format lisible, utilisez l'option `-lh` :
        ```bash
        ls -lh
        ```

10. **Changer le répertoire courant.**
      - Tapez la commande suivante pour aller dans le répertoire `/home` et appuyez sur Entrée :
         ```bash
         cd /home
         ```
      - Tapez `pwd` pour vérifier le répertoire courant.
      - Tapez la commande suivante pour remonter d'un niveau dans l'arborescence des répertoires et appuyez sur Entrée :
         ```bash
         cd ..
         ```
      - Tapez `pwd` pour vérifier le répertoire courant.
      - Tapez la commande suivante pour aller directement au répertoire personnel de l'utilisateur et appuyez sur Entrée :
         ```bash
         cd ~
         ```
      - Tapez `pwd` pour vérifier le répertoire courant.

11. **Créer un nouveau répertoire.**
      - Tapez la commande suivante et appuyez sur Entrée :
         ```bash
         mkdir Projets
         ```
      - Tapez `ls` pour vérifier que le répertoire a été créé.

12. **Supprimer le nouveau répertoire créé au #11.**
      - Tapez la commande suivante et appuyez sur Entrée :
         ```bash
         rmdir Projets
         ```
      - Tapez `ls` pour vérifier que le répertoire a été supprimé.

13. **Supprimer des fichiers ou des répertoires.**
      - Créez des fichiers pour l'exercice :
         ```bash
         touch fichier1.txt fichier2.txt
         ```
      - Tapez la commande suivante pour supprimer un fichier et appuyez sur Entrée :
         ```bash
         rm fichier1.txt
         ```
      - Tapez `ls` pour vérifier que le fichier a été supprimé.
      - Tapez la commande suivante pour forcer la suppression d'un fichier sans confirmation et appuyez sur Entrée :
         ```bash
         rm -f fichier2.txt
         ```
      - Tapez `ls` pour vérifier que le fichier a été supprimé.

14. ** Copier des fichiers ou des répertoires.**
      - Créez un fichier pour l'exercice :
         ```bash
         touch fichier.txt
         ```
      - Tapez la commande suivante pour copier un fichier et appuyez sur Entrée :
         ```bash
         cp fichier.txt copie_fichier.txt
         ```
      - Tapez `ls` pour vérifier que le fichier a été copié.
      - Créez un répertoire pour l'exercice :
         ```bash
         mkdir dossier
         ```
      - Tapez la commande suivante pour copier un fichier dans un répertoire et appuyez sur Entrée :
         ```bash
         cp fichier.txt dossier/
         ```
      - Tapez `ls dossier` pour vérifier que le fichier a été copié dans le répertoire.

15. **Déplacer ou renommer des fichiers ou des répertoires.**
      - Tapez la commande suivante pour renommer un fichier et appuyez sur Entrée :
         ```bash
         mv fichier.txt nouveau_nom.txt
         ```
      - Tapez la commande pour vérifier que le fichier a été renommé.

      - Tapez la commande suivante pour déplacer un fichier dans un répertoire et appuyez sur Entrée :
        ```bash
        mv nouveau_nom.txt dossier/
        ```

      - Tapez la commande pour vérifier que le fichier a été déplacé dans le répertoire.