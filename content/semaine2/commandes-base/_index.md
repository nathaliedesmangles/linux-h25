+++
title = "Commandes de navigation de base sous Linux"
weight = 23
+++


Naviguer dans le système de fichiers Linux est une compétence essentielle pour tout utilisateur. Dans cette leçon vous apprendrez sur les commandes de base qui vous permettront de vous déplacer et de gérer les fichiers et répertoires dans un environnement Linux.

## Commandes de base

1. **pwd (print working directory)**
   - **Description** : Affiche le chemin complet du répertoire courant.
     ```bash
     pwd
     ```
   - **Exemple de résultat** :
     ```bash
     /home/utilisateur
     ```

2. **ls (list)**
   - **Description** : Liste les fichiers et répertoires dans le répertoire courant.
     ```bash
     ls
     ```
   - **Options courantes** :
     - `ls -l` : Affiche les détails des fichiers et répertoires (permissions, propriétaire, taille, etc.).
     - `ls -a` : Affiche tous les fichiers, y compris les fichiers cachés (ceux commençant par un point).
     - `ls -lh` : Affiche les tailles de fichiers dans un format lisible (Ko, Mo, Go).
   - **Exemple** :
     ```bash
     ls -l
     total 12
     drwxr-xr-x 2 utilisateur utilisateur 4096 jan  1 12:00 Documents
     -rw-r--r-- 1 utilisateur utilisateur  123 jan  1 12:00 fichier.txt
     ```

3. **cd (change directory)**
   - **Description** : Change le répertoire courant.
     ```bash
     cd /chemin/vers/repertoire
     ```
   - **Commandes utiles** :
     - `cd ..` : Remonte d'un niveau dans l'arborescence des répertoires.
     - `cd ~` : Va directement au répertoire personnel de l'utilisateur.
     - `cd -` : Revient au répertoire précédent.
   - **Exemple** :
     ```bash
     cd /home/utilisateur/Documents
     ```

4. **mkdir (make directory)**
   - **Description** : Crée un nouveau répertoire.
     ```bash
     mkdir nom_du_repertoire
     ```
   - **Exemple** :
     ```bash
     mkdir Projets
     ```

5. **rmdir (remove directory)**
   - **Description** : Supprime un répertoire vide.
     ```bash
     rmdir nom_du_repertoire
     ```
   - **Exemple** :
     ```bash
     rmdir Projets
     ```

6. **rm (remove)**
   - **Description** : Supprime des fichiers ou des répertoires.
     ```bash
     rm nom_du_fichier
     ```
   - **Options courantes** :
     - `rm -r` : Supprime un répertoire et son contenu de manière récursive.
     - `rm -f` : Force la suppression sans demander de confirmation.
   - **Exemple** :
     ```bash
     rm fichier.txt
     rm -r dossier
     ```

7. **touch**
   - **Description** : Crée un nouveau fichier vide ou met à jour l'horodatage d'un fichier existant.
     ```bash
     touch fichier.txt
     ```
   - **Exemple** :
     ```bash
     touch fichier.txt
     ```
   - **Résultat** :
     ```plaintext
     (Aucun résultat visible, mais le fichier est créé ou mis à jour)
     ```

8. **echo**
   - **Description** : Affiche une ligne de texte ou une variable à l'écran ou dans un fichier.
     ```bash
     echo "Bonjour, ceci est un test." > fichier.txt
     ```
   - **Exemple** :
     ```bash
     echo "Bonjour, ceci est un test." > fichier.txt
     ```
   - **Résultat** :
     ```plaintext
     (Le texte "Bonjour, ceci est un test." est écrit dans le fichier fichier.txt)
     ```

9. **cp (copy)**
   - **Description** : Copie des fichiers ou des répertoires.
     ```bash
     cp source destination
     ```
   - **Options courantes** :
     - `cp -r` : Copie un répertoire et son contenu de manière récursive.
   - **Exemple** :
     ```bash
     cp fichier.txt copie_fichier.txt
     cp -r dossier copie_dossier
     ```

10. **mv (move)**
   - **Description** : Déplace ou renomme des fichiers ou des répertoires.
     ```bash
     mv source destination
     ```
   - **Exemple** :
     ```bash
     mv fichier.txt nouveau_nom.txt
     mv dossier /nouveau/chemin/
     ```

