# Mon dossier des exercices et projets pour le cours ICS3U

Voici une courte liste pour les **questions fréquentes** :

Comprendre Git et GitHub

* Voir le site du cours : [https://physcrowley.github.io/ICS3U/1-Bases](https://physcrowley.github.io/ICS3U/1-Bases)
* Voir la section pertinente de la [documentation pour VS Code](https://code.visualstudio.com/docs/editor/github#_setting-up-a-repository) - ignorer les détails sur les Suggestions, Pull Requests et Issues. On ne s'en servira pas.

Trouver les exercices à faire

* Voir le [site du cours](https://physcrowley.github.io/ICS3U) au bas de chaque section pour les questions
* Voir Google Classroom pour les détails spécifiques sur comment rendre le travail

Trouver la rétroaction sur mon travail

* Aller dans mon compte GitHub à l'onglet `Issues` *(ok... oui, on va se servir des Issues, mais on va se rendre sur GitHub pour le faire)*

## Quoi faire en premier avec ce répertoire

La première étape, dès que vous recevez votre copie de ce répertoire (dossier), est de le **clôner** sur votre propre machine pour y avoir accès dans VS Code.

> Vous devez avoir Git sur votre système avant de commencer cette étape. Si vous êtes sur Coding Rooms, Git est déjà installé.

1. Sur GitHub, à l'onglet `<> Code`, copier l'addresse du répertoire.
2. Ouvrir VS Code (sur votre machine ou avec un workspace sur Coding Rooms).
    > Le workspace sur *Coding Rooms* doit utiliser l'environnement Visual Studio Code (pas CR2). Voir les notes de cours, [section installation]([https://physcrowley.github.io/ICS3U/1-Bases]) pour les détails sur comment le préparer.
4. Ouvrir la liste des commandes avec `Ctrl/Cmd + Maj + P` et taper "clone". Choisir l'option "Git: Clone".
5. Coller l'adresse du répertoire que vous aviez copiée de GitHub et taper `Enter`.
6. Choisir un dossier sur votre ordinateur.
     * Sur *Windows, macOS, Linux* : je suggère `<spécifique à mon système>/Documents` où la partie spécifique à votre système dépend de votre ordinateur et de votre nom d'utilisateur. Le dossier sera créer dans votre dossier "Documents" et sera donc facile à trouver.
     * Sur *Coding Rooms* : utiliser `/usercode/` afin que le dossier apparaisse automatiquement quand vous ouvrez l'espace de travail plus tard.
7. Après quelques instants, VS Code ouvre une alerte en bas à la droite de la fenêtre. Choisir "Open in new Window".
8. Vous travaillez maintenant dans ce dossier sur VS Code et vous pouvez ajouter et modifier les fichiers et les dossiers, exécuter les programmes, etc.

## Ouvrir ce dossier dans le futur

> Sur Coding Rooms, le dossier sera présent chaque fois que vous ouvrez à nouveau le workspace.

1. Ouvrir VS Code.
2. Choisir d'ouvrir un dossier (`Ctrl + K` suivi de `Ctrl + O` ou `File > Open folder`)
3. Naviguer au dossier avec l'explorateur et cliquer OK.

## Faire un changement et le synchroniser sur GitHub

La synchronisation se passe en deux étapes quand vous avez travaillez sur votre machine :

1. Créer une nouvelle image de la version sur votre machine, ce qui s'appelle un *commit*.
2. Pousser (*Push*) cette version vers GitHub.

### Partie 1 - Faire notre premier *commit* (ou image de version)

1. Rentrer dans le sous-dossier "exercices" en cliquant dessus dans l'Explorer de VS Code.
2. Cliquer l'icône pour créer un nouveau fichier. Le curseur sera indenté sous "exercices" si vous êtes au bon endroit.
3. Taper le nom "sync_test.txt" et `Enter` pour créer un fichier TEXT.
4. Ajouter une courte phrase, comme "Je sychronise mon ordi avec GitHub!!!" dans l'éditeur et enregistrer le fichier.
5. Cliquer sur l'icône pour la gestion des versions dans la barre d'activité. Vous verrez deux sections : *Message* et *Changes*. Vous devriez voir le nouveau fichier sous *Changes*.
6. À côté du fichier ou du titre *Changes* vous pouvez cliquer sur l'icône `+`. Une troisième section apparaît : *Staged* et votre fichier se trouve maintenant là. Cela veut dire que votre fichier fera partie de la nouvelle image de version (le nouveau *commit*).
    * Le `+` à côté de *Changes* ajoute tous les fichiers disponibles au prochain *commit* tandis que le `+` à côté des fichiers vous permet d'ajouter les fichiers individuellement.
7. Il ne reste qu'à taper un court message (<50 caractères) pour indiquer quel changement est à synchroniser, p. ex. "ajouter un fichier de test de synchronisation", et de cliquer sur le `✔`. Le crochet lance le *commit* et le fichier disparaît parce l'état du dossier est maintenant identique à l'état du dernier *commit*.

Pour les prochains *commit*, ce sont les étapes 5 à 7 qui se répètent. Cela deviendra très routinier avec la pratique.

### Partie 2 - Synchroniser avec GitHub

1. À la barre d'état au bas de la fenêtre de VS Code, vous verrez tout à gauche le symbole des versions avec le mot `main` qui signifie que nous sommes sur la branche `main` de notre dossier. Immédiatement à la droite vous verrez différentes flèches selon l'état de synchronisation.
    * S'il n'y a rien à synchroniser, ce sera deux flèches en cercle, un peu comme `🔄`.
    * S'il y a des changements sur votre ordi qui ne sont pas sur GitHub, vous verrez quelque chose comme `⬇0 ⬆2` pour indiquer qu'on a quelque chose à envoyer.
    * S'il y a des changements sur GitHub qui ne sont pas sur votre ordi, vous verrez quelque chose comme `⬇3 ⬆0` pour indiquer qu'il y a quelque chose à télécharger.
2. Les changements faits sur votre ordi sont seulement indiqués s'il y a un *commit*, donc les chiffres représentent le nombre de *commits* depuis la dernière synchronisation.
3. Pour faire la synchronisation, il suffit de **cliquer sur ces flèches** et d'attendre quelques instants.

La **première fois** que vous faites une synchronisation, VS Code vous demandera de vous **authentifier avec GitHub**. Simplement suivre les instructions. Cela vous aménera sur GitHub et de retour à VS Code. Ça peut prendre quelques tentatives la première fois, alors soyez attentifs et patients.

* Sur *Coding Rooms*, il faut s'identifier chaque fois qu'on ouvre le workspace.
* Sur *Coding Rooms*, TRÈS IMPORTANT : quand l'alerte apparaît pour vous demander de vous rendre sur le site de GitHub, il faut :
    1. Cliquer sur "Copy" (pas sur "Open").
    2. Ouvrir un nouvel onglet et coller le lien. Ensuite taper `Enter`.
    3. Compléter le processus en suivant les instructions.

### Dernier mot 

> Rappelez vous que c'est un processus en deux étapes.

*  Si vous ne créez pas de *commits*, alors il n'y a rien à synchroniser. VS Code vous aide avec ça en fournissant un rappel visuel : s'il y a des changements qui ne font pas partis d'un *commit*, le mot `main` dans la barre d'état devient `main*`.
* Si vous ne synchronisez pas les *commits* que vous avez fait, vous n'aurez pas accès à votre travail sur GitHub (et donc sur le web) et l'enseignant non plus. Alors, si le symbole de synchronisation n'est **pas** `🔄` avant d'arrêter le travail, il faut synchroniser avant de terminer.