## **Définition**

Le terminal ou plus communément appelé : « interpréteur de commandes » est un logiciel système faisant partie des composantes de base d’un système d’exploitation. Sa fonction est donc d’interpréter les commandes qu’un utilisateur tape au clavier dans l’interface en ligne de commande. Celui-ci permet de « parler » à son ordinateur.

En anglais le terminal est appelé : « command-line interpreter », le CLI.

Le terminal est une version un peu moins intuitive qu’un explorateur fichier normal mais beaucoup plus puissant. En effet, le terminal nous permet de parler directement à votre ordinateur, tandis que l’explorateur de fichier est une surcouche du terminal.

C’est donc une version texte de l’explorateur de fichier « graphique ».
	 - CLI = command line interface = terminal = version texte de l’explorateur.
	 - GUI = graphical user interface = explorateur fichier = version comme on la connaît. vv

## **Comment lancer le terminal ?**

Selon l'ordinateur que vous possédez, différente manière existe pour lancer le terminal : MacOS et Linux utilisent le même noyau de système d’exploitation qui est Unix. Windows lui, utilise DOS. Le terminal *Shell Unix* est installé de base pour les MacOS et Linux. Windows devra trouver une alternative à l'invite de commande, ici proposée : *Cygwin*.

- Sous MacOS faire CMD + SPACE, puis écrire Terminal (ou iTerm), Enter
- Sous Linux, faire CTRL + ALT + T
- Sous Window, installer Cygwin

## **Les premières fonctions**

Pour faire marcher le terminal : il suffit de rentrer le texte correspondant à une fonction pour que celle-ci s’exécute. Lorsque dans un explorateur en GUI il suffit de double cliquer sur un fichier ou dossier pour l’ouvrir, il faudra taper dans le terminal que l’on veut ouvrir tel fichier ou tel dossier pour qu’il le fasse.

Si tu exécutes la commande : *echo « Hello world »*, le terminal te renvoie **_Hello world !_** C’est ainsi qu’est créée la première interaction avec l’ordinateur, via une commande du terminal.

* **La commande PWD** :

*pwd* est l’acronyme de Print Working Directory. Cette commande sert à afficher dans quel dossier tu te trouves. C’est généralement la première commande que l’on tape lorsque l’on arrive dans le terminal de quelqu’un, pour pouvoir s’y retrouver.

Si j’exécute la commande *pwd*, le terminal me renvoie **/usr/bin**.

* **La commande LS**:

*l*s est le diminutif de list. Cette fonction sert à afficher les fichiers et les dossiers situés dans le dossier dans lequel je me trouve actuellement

-- *ls -a*  à dossiers et fichiers commençant par « . »
-- *ls -l*  à dossiers et fichiers au format long
-- *ls -al*  à dossiers et fichiers au format long et commençant par « . »

On peut donc ajuster les options aux fonctions en utilisant : fonction -option.

*  **La commande MAN**: 

*man* est le diminutif de manual. Cette commande lance le manuel d’une fonction précise afin de connaître toutes ses spécificités. Il faut ainsi taper : man fonction.

-- man ls
-- man pwd

Cette commande ouvre le manuel de la fonction tapée, il suffit de taper *q* pour quitter.

* **La commande CD**:

La notion de géographie est importante, tout comme dans l’explorateur en GUI où l’on se déplace de dossiers en dossiers en double-cliquant, sur le terminal on se déplace aussi. Pour ceci on utilise la commande *cd*.

*cd* est l’acronyme de *Change Directory*. Cette commande permet donc ne naviguer de dossiers en dossiers équivalant à un double-clique sur un dossier.

-- *cd nomdudossier*
-- *cd ..* à Cette commande te permet de revenir en arrière, dans le dossier précédent

La touche **TAB**, se situant au-dessus de la touche de verrouillage de la majuscule qui peut être représentée par deux flèches à sens inverses permet de faire de l’autocomplétion et d’afficher les dossiers disponibles si l’on fait : *cd + [SPACE] + TAB + TAB*.

Pour quitter cette fonction, il suffit de taper *q*.

* **La commande MKDIR**:

*mkdir* permet de créer un dossier en tapant : *mkdir nomdudossier*

* **La commande TOUCH** :

*touch* permet de créer un fichier en tapant : *touch nomdufichier*

* **La commande MV**:

*mv* permet de couper, c’est-à-dire de déplacer un fichier ou dossier d’un endroit vers un autre, en rentrant : *mv [fichier_à_couper] [lieu_de_destination]*

*mv* étant le diminutif de *move*, permet également de renommer un fichier. En effet il suffit de taper : *mv ancien_nom_de_fichier nouveau_nom_de_fichier*

* **La commande RM**:

*rm* accronyme de *remove* permet de supprimer un fichier :

-- *rm nomdufichier*

Il permet aussi de supprimer un dossier et son contenu en ajoutant *-r* comme « recursion » en option :

-- *rm -r nomdudossier*

**ATTENTION !** Si tu tapes rm -rf /  ou rm -rf * dans ton terminal, cela lui ordonne de tout effacer, en forçant les barrières. Ainsi, ceci indique que tout le contenu de l’ordinateur va être supprimé. *rm* étant très rapide, l’intégralité de l’ordinateur est effacé en quelques secondes, ainsi **ne faut JAMAIS le faire !**

* **VIM** :

Vim est un éditeur de texte passant uniquement par le terminal. Ainsi il utilise tout comme le terminal simplement le clavier. Pour y accéder il suffit de taper : *vim nomdufichier* et ainsi cela ouvrira vim sur le fichier indiqué et permettra de l’éditer.

Pour quitter vim il faut entrer : *q !*

* **Astuces** 

-- *CTRL + C* à annule la fonction en cours
-- *CTRL + U*  à efface la ligne en cours
-- Les flèches du haut et du bas permettent de naviguer dans l’historique des commandes
-- Il est possible de pimper son terminal, d’ajouter des couleurs grâce au cours de Viking Code School.
