+++
title = "Exécution de commandes à l’aide du Shell Bash"
weight = 21
+++

Le shell Bash (*Bourne Again SHell*) est un interpréteur de commandes utilisé principalement sur les systèmes d'exploitation Unix et Linux. Il permet aux utilisateurs d'exécuter des commandes pour interagir avec le système d'exploitation, automatiser des tâches et gérer des fichiers et des processus. Cette leçon se concentre sur l'exécution de commandes simples à l'aide du shell Bash.


## La ligne de commande

1. **Ligne de commande**:
   - La ligne de commande est l'interface où vous tapez vos commandes. Elle est souvent représentée par un symbole `$` ou `#` pour les utilisateurs root.
   - Lorsque vous êtes prêt à exécuter une commande, appuyez sur la touche Entrée. Tapez chaque commande sur une ligne séparée. Le résultat de la commande est affiché avant l’invite du shell suivante.

**Exemple**:
```plaintext
[user@host]$ whoami
user
[user@host]$ 
```

## Commandes simples

Ces commandes simples sont essentielles pour naviguer et gérer efficacement un système Linux à l'aide du shell Bash. La maîtrise de ces commandes vous permettra d'effectuer des tâches courantes de manière plus efficace et de mieux comprendre le fonctionnement de votre système.

1. **date**
   - **Description** : Affiche ou définit la date et l'heure du système.
     ```bash
     date
     ```
   - **Résultat** :
     ```bash
     Mon Dec  3 11:45:00 EST 2024
     ```

2. **passwd**
   - **Description** : Change le mot de passe de l'utilisateur.
     ```bash
     passwd
     ```
   - **Résultat** :
     - L'utilisateur est invité à entrer son mot de passe actuel, puis le nouveau mot de passe.

3. **cat**
   - **Description** : Affiche le contenu d'un fichier ou concatène plusieurs fichiers.
     ```bash
     cat nom_du_fichier
     ```
   - **Exemple** :
     ```bash
     cat fichier.txt
     ```
   - **Résultat** :
     ```plaintext
     Contenu du fichier.txt
     ```

4. **less**
   - **Description** : Affiche le contenu d'un fichier page par page.
     ```bash
     less nom_du_fichier
     ```
   - **Exemple** :
     ```bash
     less fichier.txt
     ```
   - **Navigation** :
     - `Espace` : Page suivante
     - `b` : Page précédente
     - `q` : Quitter

5. **head**
   - **Description** : Affiche les premières lignes d'un fichier.
     ```bash
     head nom_du_fichier
     ```
   - **Options courantes** :
     - `head -n 10 nom_du_fichier` : Affiche les 10 premières lignes (par défaut).
   - **Exemple** :
     ```bash
     head fichier.txt
     ```

6. **tail**
   - **Description** : Affiche les dernières lignes d'un fichier.
     ```bash
     tail nom_du_fichier
     ```
   - **Options courantes** :
     - `tail -n 10 nom_du_fichier` : Affiche les 10 dernières lignes (par défaut).
     - `tail -f nom_du_fichier` : Affiche les nouvelles lignes ajoutées en temps réel.
   - **Exemple** :
     ```bash
     tail fichier.txt
     ```

7. **; (point-virgule)**
   - **Description** : Permet d'exécuter plusieurs commandes sur une seule ligne.
     ```bash
     commande1 ; commande2
     ```
   - **Exemple** :
     ```bash
     date ; whoami
     ```
   - **Résultat** :
     ```plaintext
     Mon Dec  3 11:45:00 EST 2024
     utilisateur
     ```

8. **wc**
   - **Description** : Compte les lignes, mots et caractères d’un fichier. Accepte les options -l, -w ou -c pour n’afficher respectivement que le nombre de lignes, de mots ou de caractères.
     ```bash
     [user@host ~]$ wc /etc/passwd
     45  102 2480 /etc/passwd
     ```
   - **Exemple** :
     ```bash
     [user@host ~]$ wc -l /etc/passwd ; wc -l /etc/group
     45 /etc/passwd
     70 /etc/group
     ```
   - **Résultat** :
     ```plaintext
     45 /etc/passwd
     70 /etc/group
     ```

9. **tabulation**
   - **Description** : Permet de compléter rapidement les commandes et les noms de fichiers après avoir entré un nombre de caractères suffisant pour réduire les possibilités à une seule. Si les caractères saisis ne sont pas uniques, appuyez deux fois sur la touche de tabulation pour afficher toutes les commandes correspondantes.
     ```bash
     [user@host ~]$ pas Tab+Tab
     passwd       paste        pasuspender
     [user@host ~]$ pass Tab
     [user@host ~]$ passwd 
     Changing password for user user.
     Current password: 
     ```
   - **Exemple** :
     ```bash
     [user@host ~]$ ls /etc/pas1Tab
     [user@host ~]$ ls /etc/passwd2Tab
     passwd   passwd-
     ```
   - **Résultat** :
     ```plaintext
     passwd
     passwd-
     ```

10. **history**
   - **Description** : Affiche la liste des commandes précédemment exécutées, précédées d’un numéro de commande. Le point d’exclamation (!) rappelle les commandes précédentes sans avoir à les retaper. La commande **`!number`** rappelle la commande correspondant au nombre spécifié. La commande **`!string`** rappelle la commande la plus récente qui commence par la chaîne spécifiée.
     ```bash
     [user@host ~]$ history
     ...output omitted...
     23  clear
     24  who
     25  pwd
     26  ls /etc
     27  uptime
     28  ls -l
     29  date
     30  history
     ```
   - **Exemple** :
     ```bash
     [user@host ~]$ !ls
     ls -l
     total 0
     drwxr-xr-x. 2 user user 6 Mar 29 21:16 Desktop
     ...output omitted...
     [user@host ~]$ !26
     ls /etc
     abrt                     hosts                     pulse
     adjtime                  hosts.allow               purple
     aliases                  hosts.deny                qemu-ga
     ...output omitted...
     ```
   - **Résultat** :
     ```plaintext
     ls -l
     total 0
     drwxr-xr-x. 2 user user 6 Mar 29 21:16 Desktop
     ls /etc
     abrt                     hosts                     pulse
     adjtime                  hosts.allow               purple
     aliases                  hosts.deny                qemu-ga
     ```