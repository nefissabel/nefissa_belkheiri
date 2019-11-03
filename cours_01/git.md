## Définition Git et GitHub
Git est un outil très connue par les programmeurs : c’est un logiciel de gestion de versions. Il va permettre de versionner votre code, c’est à dire, de garder une trace de toutes les modifications faite sur votre code : on appel ça un “commit”. Le commit est donc une série de modification sur l’ensemble des fichiers du projets (création, suppression, ajout de texte ect…). Chacun de ces commit créer, est ce que l’on appel une version du code, et on peut la consulter à n’importe qu’elle moment. On peut donc savoir quels fichiers ont étés modifié, quand, qui, et pourquoi. Avec ce genre de logiciel, on peut travail en groupe, beaucoup plus simplement. Par exemple, sur un projet de site web, plus le projet évolue, plus des modifications vont être faite : grâce au commit, on pourra avoir un historique de toutes ces modifications.

  

Github, est donc un service en ligne qui utilise le système de Git. Il permet donc aux utilisateurs de mettre en ligne ses dossiers Git (nous verrons plus tard comment le faire), et permet d’avoir plusieurs personnes (collaborateurs) sur un même dossiers Git.

## Installer Git
Maintenant que nous avons compris qu’est ce qu’est Git, nous allons voir comment l’installer sur notre ordinateur. Pour pouvoir utilisez Git, nous aurons besoin d’utiliser la console / le terminal (cf cours sur le terminal).

- **SOUS MAC ET LINUX**

Pour installer le logiciel c’est très simple : il suffit de le telercharger, via le site de Git ([cliquez ici](**[http://git-scm.com/downloads](http://git-scm.com/downloads)**)). Une fois installé, il suffit de lancer son terminal, et exécuter les commandes suivantes :

-- *git config - -global user.name "Votre nom ou pseudo"*

-- *git config - -global user.email "Votre email"*

C’est 2 premières commandes permet de se créer un compte gratuit sur Github.

Par la suite, on peut faire la commande *“git --version”*, qui nous permet de vérifier que le Git a bien été installé.

- **SOUS WINDOWS**

Il faut télécharger le logiciel sur le lien suivant : [cliquez ici](**[http://msysgit.github.io](http://msysgit.github.io)**).  Etant donné que sous Window, il n’y a pas forcément toute les commandes du terminales “classique” (ls, cd, mkdir…), comme sous MacOs ou Linux, ce lien va nous permettre de également de générer une console émulant le comportement de Bash, la console sous Linux. 
Une fois le logiciel installé, il suffit de reproduire les mêmes commandes que pour Mac et Linux.

Tout est prêt, on peut donc s'intéresser à la mise en place d’un dossier (un repository).

**ATTENTION !** avant toute chose, il faut avoir un dossier que l’on souhaite “copié” sur le GitHub. On va donc créer un dossier, via le terminal, grâce au commande mkdir, cd et touch (cf cours sur le terminal). Ce dossier ne peut pas être "Mes Documents" ou "Bureau".

## Manipulation du dossier (étape par étape)

- **git init et git status**

Une fois le dossier créer, il faut initialiser Git dedans, c’est a dire dire au logiciel Git, que l’on a précédemment télécharger, que CE dossier est un projet, ce qui permettra de faire des commits plus tard (donc l’activer comme étant un repository GIT).

  

Pour ce faire, il suffit d’utiliser la commande *“ git init”*. Une fois que c’est fait, la commande *“git status”* nous permettra de voir l’état du projet git, c’est a dire qu’elle dossier on aura ajouter et attend d’être commits ( apparaît en vert), ou au contraire, ce qui n’ont pas du tout été ajouté (apparaît en rouge).

- **git remote**

Après avoir dit au logiciel Git qu’elle dossier est un repository, il faut lier le dossier présent sur l’ordinateur, au repository que l’on aura précedemment créé sur Github :

*“git remote add origin git @ github .com:nom_utilisateur/nom_repository.git*”

- **git add**

Cette commande permet de dire quel fichier nous souhaitons commits plus tard, il suffit de faire : “git add nom_du_fichier_ou_dossier” (on peut vérifier par la suite grâce à git status, que le fichier apparaît en vert et que donc, il attend d’être commit).

**PETITE ASTUCE** : si l'on souhaite  add un dossier qui est vide, Git ne pourra pas le faire. Après avoir créer le dossiers (grâce a la commande mkdir), il faut : *touch nomdudossier/.gitignore* puis à partir de la, on peut le add normalement (*git add nomdudossier*).

- **git commit**

La fameuse commande qui nous intéresse : commit. C’est très simple, cette commande permet donc de “prendre en photo”, le fichier/dossier que l’on souhaite (que si on l’as git add juste avant). Il faut donc faire : *“git commit -m “commentaire souhaité”*. Ainsi, tout les fichier/dossier apparut en vert dans le git status, on été pris en photo sous le commentaire que l’on a rentré. Si on refait *git status*, on remarque que c’est fichier ne sont plus en vert ou en rouge.

Une fois que tous les dossiers ont été add et commits (donc plus aucun fichier/dossier en rouge ou en vert), si on refait *git status*, ca nous affiche donc *“nothing to commit, working tree clean”*.

- **git log**

Grâce à cette commande, on peut donc voir la liste de tous les commits que l’on a faits au cours du projet. Plusieurs détails s’affichent, tels que l’auteur du commit, la date, ou même le commentaire que l’a personne a rentrée lors du commit.

- **git push et git pull**

Maintenant, il faut que vous envoyer votre code présent dans les fichiers sur le GitHub.
Sur le terminal, il faut donc entrer : *“git push origin master”*.
Git comprend donc qu'il faut envoyer le code que contient la branche master, vers le remote GitHub, appelé origin.
Une fois que c’est fait, vous pouvez allez consulter les commits sur le site de GitHub.  

Pour faire l’inverse, il suffit de faire : *“git pull origin master”*.
