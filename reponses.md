B1-Git - Partie 1 : Création du dépôt et commits
Ouvrir un terminal (terminal Git Bash à privilégier)
->executé Git Bash en administrateur.

Créer, en ligne de commande, un répertoire tp-git
-> mkdir tp-git

Se déplacer dans le répertoire
-> cd tp-git

Vérifier qu'on est dans le bon répertoire en affichant le chemin du répertoire courant
-> pwd. Il affiche /c/Users/Noa/OneDrive - Notre Dame de Grace/Bureau/cours/Gahide/tp-git/

Initialiser un dépôt Git
-> git init

Lister tous les fichiers du répertoire (y compris les fichiers cachés) pour s'assurer que le répertoire .git à été créé
->ls -a

Ouvrir ce répertoire sous VS Code
-> il faut aller dans File, Open Folder... et choisir le dossier tp-git

Exécuter git status et copier/coller la sortie
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        reponses.md

nothing added to commit but untracked files present (use "git add" to track)



Créer le fichier fichier1.md avec un contenu quelconque et l'enregistrer (vous pouvez utiliser VS Code pour créer et éditer des fichiers)
->touch fichier1.md

Attention, il s'agit bien de créer un nouveau fichier, et non un répertoire. Il en sera de même tout au long de ce TP.
Créer le fichier fichier2.md avec un contenu quelconque et l'enregistrer
->touch fichier2.md

Exécuter git status et copier/coller la sortie
-> On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier1.md
        fichier2.md
        reponses.md

nothing added to commit but untracked files present (use "git add" to track)


Ajouter fichier1.md à l'index de Git (zone de Staging)
-> git add fichier1.md

Exécuter git status et copier/coller la sortie
->On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   fichier1.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier2.md
        reponses.md


Créer un commit avec pour message : "Ajout de fichier1.md"
->git commit -m "Ajout de fichier1.md"





VALIDATION PROF01





Exécuter git status et copier/coller la sortie
->On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier2.md
        reponses.md

nothing added to commit but untracked files present (use "git add" to track)



Modifier fichier1.md et enregistrer


Exécuter git status et copier/coller la sortie
->On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   fichier1.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        fichier2.md
        reponses.md

no changes added to commit (use "git add" and/or "git commit -a")


Ajouter fichier1.md et fichier2.md à la zone de Staging
-> git add fichier1.md fichier2.md

Créer un commit "Ajout de fichier2.md et modification de fichier1.md"
->git commit -m "Ajour de fichier2.md et modification de fichier1.md

 
Exécuter git status et copier/coller la sortie
->On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        reponses.md

nothing added to commit but untracked files present (use "git add" to track)


Copier/coller l'ID des deux premiers commits (utiliser log) :

ID commit 1 :6e6efc122e775f4e973d1d8412a833589e05f4d7
ID commit 2 :790e67709bff292434f8526fdf51cf6931fd45a2

Que signifie qu'un fichier est "tracked" ou "untracked" ?
->tracked veut dire que le fichier est suivie par git et untracket c'est que le fichier n'a pas d'importance pour git

Pourquoi doit-on passer les fichiers par la zone de Staging (l'index) avant de les committer ?
-> Pour choisir ce qu'on veut commit ou pas.



VALIDATION PROF02


