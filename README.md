# Learn-Git
### Objectifs :
- Comprendre ce qu'est GitHub.
- Savoir pourquoi GitHub est important pour les développeurs.
- Apprendre les concepts de base de GitHub.

### Qu'est-ce que GitHub ?
GitHub est une plateforme de gestion de versions basée sur le cloud qui permet aux développeurs de collaborer sur des projets, de suivre l'évolution des codes sources et de gérer efficacement les modifications apportées à un projet. Il est largement utilisé dans le développement logiciel, mais peut également être utilisé pour d'autres types de projets.

### Why Git:
#### Gestion de versions : 
GitHub utilise le système de contrôle de version Git, qui permet de suivre chaque modification apportée au code source. Cela permet de revenir en arrière en cas d'erreur et de fusionner facilement les contributions de plusieurs développeurs.

#### Collaboration : 
Plusieurs personnes peuvent travailler sur le même projet simultanément, en fusionnant leurs modifications de manière transparente. Cela facilite la collaboration sur des projets open source et en équipe.

#### Suivi des problèmes : 
GitHub permet de signaler et de suivre les problèmes, les bogues et les demandes de fonctionnalités. Cela facilite la gestion des tâches et des problèmes liés au projet.

#### Documentation : 
Vous pouvez héberger la documentation de votre projet sur GitHub, ce qui la rend facilement accessible à tous les contributeurs et aux utilisateurs du projet.

### Concepts importants :
1. **Dépôt** (Repository) : Un dépôt est un espace où vous stockez votre code source. Il peut s'agir d'un projet individuel ou d'un projet partagé avec d'autres développeurs.
2. **Clone** : Faire un clone d'un dépôt signifie copier le code source depuis un dépôt distant (sur GitHub) vers votre propre machine locale pour y travailler.
3. **Commit** : Un commit est une modification apportée au code source, accompagnée d'un message qui décrit la modification. Les commits sont utilisés pour enregistrer l'historique des modifications.
4. **Pull Request** : Une pull request est une demande d'intégration de vos modifications dans le dépôt principal. Cela permet aux autres contributeurs de passer en revue vos modifications avant de les fusionner.
5. **Branch (Branche)** : Une branche est une version isolée du code source. Vous pouvez créer des branches pour travailler sur des fonctionnalités ou des correctifs sans affecter la branche principale.
6. **Merge (Fusionner)** : Fusionner signifie intégrer les modifications d'une branche dans une autre. Les pull requests sont généralement utilisées pour fusionner des branches.
7. **Fork (Fourche)** (pas couvert) : Une fourche est une copie d'un dépôt sur lequel vous avez un contrôle total. Vous pouvez apporter des modifications à votre propre copie et proposer des pull requests pour les intégrer au dépôt d'origine.

## GitBash
Git Bash est un terminal qui offre une interface en ligne de commande pour travailler avec Git. Voici comment commencer à l'utiliser :
- **Téléchargement et installation** : Si vous n'avez pas encore installé Git Bash, vous pouvez le télécharger depuis le site officiel de Git (https://git-scm.com/). Suivez les instructions d'installation pour votre système d'exploitation.
- **Lancement de Git Bash** : Une fois installé, lancez Git Bash à partir du menu de démarrage ou en le cherchant dans les applications installées.
- **Configuration initiale** : Avant de commencer à utiliser Git Bash, vous devez configurer votre nom d'utilisateur et votre adresse e-mail pour identifier vos commits. Utilisez les commandes suivantes pour configurer Git avec vos informations :

     ```
     git config --global user.name "Votre nom"
     git config --global user.email "votre@email.com"
     ```
- **Clonage d'un dépôt** : Pour cloner un dépôt existant depuis GitHub vers votre machine locale, utilisez la commande git clone suivie de l'URL du dépôt. Par exemple :
    ```
    git clone https://github.com/nom_utilisateur/nom_du_depot.git
    ```
- **Navigation dans les répertoires** : Vous pouvez utiliser des commandes telles que cd pour naviguer vers le répertoire où vous avez cloné un dépôt.

- **Utilisation de Git** : Vous pouvez maintenant utiliser Git Bash pour effectuer diverses opérations Git, telles que la création de branches, l'ajout de fichiers, la réalisation de commits et la création de pull requests. Voici quelques commandes couramment utilisées :
  - git status : Affiche l'état actuel de votre répertoire de travail et des fichiers modifiés.
  - git add : Ajoute des fichiers modifiés ou nouvellement créés à la zone de préparation (staging area) pour le prochain commit.
  - git commit : Crée un commit avec les modifications dans la zone de préparation.
  - git push : Envoie vos commits vers le dépôt distant (sur GitHub).
  - git pull : Récupère les modifications depuis le dépôt distant vers votre copie locale.
  - git branch : Affiche la liste des branches dans votre dépôt.

    Déconnexion : Pour quitter Git Bash, vous pouvez simplement fermer la fenêtre du terminal ou utiliser la commande exit.

## Première importation
3 manières de récupérer un projet en cours

- À l'aide de la clé SSH
- À l'aide de la clé https
- À l'aide d'un GUI externe ou d'un IDE

### par clé https 
1. Obtenez l'URL HTTPS du référentiel :
- Allez sur la page du référentiel GitHub que vous souhaitez importer.
- Cliquez sur le bouton vert "Code" en haut à droite, à côté du bouton "Watch" et "Star".
- Sélectionnez "HTTPS" si ce n'est pas déjà sélectionné. Copiez l'URL qui apparaît.

2. Ouvrez Git Bash :
    - Ouvrez Git Bash sur votre ordinateur. Assurez-vous que Git est installé et configuré correctement (comme expliqué précédemment dans ce cours).

3. Naviguez vers le répertoire où vous souhaitez importer le référentiel :
- Utilisez la commande cd pour vous déplacer vers le répertoire où vous souhaitez que le référentiel soit cloné. Par exemple, pour aller dans le dossier "Projets", vous pouvez saisir :
```
cd Chemin/Vers/Votre/Répertoire/Projets
```

4. Clonez le référentiel :
- Utilisez la commande git clone suivie de l'URL HTTPS que vous avez copiée à l'étape 1. Par exemple :
```
git clone https://github.com/nom_utilisateur/nom_du_depot.git
```
*Remplacez nom_utilisateur par le nom d'utilisateur du propriétaire du référentiel et nom_du_depot par le nom du référentiel que vous souhaitez cloner.*

5. Authentification (si nécessaire) :
- Si le référentiel est privé, Git Bash peut vous demander de vous authentifier. Vous devrez saisir votre nom d'utilisateur GitHub et votre mot de passe (ou un jeton d'accès personnel si vous l'avez configuré).

6. Attendez la fin du clonage :
- Git Bash commencera à cloner le référentiel depuis GitHub vers votre ordinateur. Attendez que le processus soit terminé. Vous verrez un message indiquant que le clonage a été réussi.

### Par GUI (GitHub desktop)
1. Téléchargez et installez GitHub Desktop :
- Si vous n'avez pas déjà GitHub Desktop installé, vous pouvez le télécharger à partir du site officiel de GitHub Desktop (https://desktop.github.com/) et l'installer sur votre ordinateur.

2. Connectez-vous à votre compte GitHub :
- Lancez GitHub Desktop après l'installation.
- Si vous n'êtes pas déjà connecté à votre compte GitHub, cliquez sur "Sign in to GitHub.com" en haut à droite de la fenêtre et suivez les instructions pour vous connecter.

3. Ouvrez l'onglet "File" (Fichier) :
- Dans GitHub Desktop, cliquez sur l'onglet "File" (Fichier) en haut à gauche de la fenêtre.

4. Sélectionnez "Clone Repository" (Cloner un dépôt) :
- Dans le menu déroulant de l'onglet "File", sélectionnez "Clone Repository" (Cloner un dépôt).

5. Choisissez le référentiel à cloner :
- Une fenêtre de recherche de référentiel apparaîtra. Vous pouvez y rechercher le référentiel que vous souhaitez importer en utilisant des mots-clés ou en parcourant vos propres référentiels GitHub.

6. Sélectionnez le référentiel :
- Une fois que vous avez trouvé le référentiel que vous souhaitez importer, cliquez dessus pour le sélectionner.

7. Configurez l'emplacement de clonage :
- Vous pouvez choisir l'emplacement où vous souhaitez que le référentiel soit cloné sur votre ordinateur. Par défaut, il utilisera un répertoire sur votre disque local, mais vous pouvez modifier cet emplacement si nécessaire.

8. Cliquez sur "Clone" (Cloner) :
- Une fois que vous avez configuré l'emplacement, cliquez sur le bouton "Clone" (Cloner) en bas à droite de la fenêtre.

9. Attendez la fin du clonage :
- GitHub Desktop commencera à cloner le référentiel depuis GitHub vers votre ordinateur. Attendez que le processus soit terminé. Vous verrez un message indiquant que le clonage a été réussi.

10. Accédez au référentiel :
- Après le clonage, vous verrez le référentiel listé dans la fenêtre principale de GitHub Desktop. Vous pouvez double-cliquer sur le référentiel pour l'ouvrir dans votre éditeur de code préféré et commencer à travailler sur le projet.
  
## Do it yourself :

Assurez-vous que vous êtes sur la branche principale : Utilisez la commande suivante pour vous assurer que vous êtes sur la branche principale de votre référentiel :

```
git branch
```

Vous devriez voir un astérisque (*) à côté de la branche principale, indiquant que vous êtes actuellement sur cette branche.

### Creation de sa branche de travail

Créez une nouvelle branche : Utilisez la commande suivante pour créer une nouvelle branche. Remplacez <nom_de_la_branche> par le nom que vous souhaitez donner à votre nouvelle branche. Par exemple, "ma-nouvelle-fonction" :
```
git branch <nom_de_la_branche>
```

Créer une autre nouvelle branche. Elle servira de branche principal fictive pour les manipulations à distance
```
git branch main_fictif_<ton_nom>
```

#### Distance vs Local
Différences entre l'environnement local et distance (remote)
Principales différences :

**Emplacement** :
   Le dépôt local se trouve sur votre ordinateur.
   Le dépôt à distance se trouve sur un serveur distant.

**Accessibilité** :
   Vous pouvez travailler sur le dépôt local même hors ligne.
   Le dépôt à distance permet la collaboration en rendant le code accessible à d'autres membres de l'équipe, généralement via Internet.

**Synchronisation** :
   Vous pouvez pousser (push) vos modifications depuis le dépôt local vers le dépôt à distance pour partager vos contributions.
   Vous pouvez tirer (pull) les modifications depuis le dépôt à distance vers le dépôt local pour intégrer les contributions des autres.

**Gestion des Contributions** :
   Le dépôt à distance est généralement utilisé pour la coordination des contributions entre plusieurs développeurs.
   Le dépôt local est votre espace de développement personnel.
        
### Changer de branch
Basculez vers la première branche créée branche : Utilisez la commande suivante pour basculer vers la nouvelle branche que vous venez de créer :

```
git checkout <nom_de_la_branche>
```

Maintenant, vous travaillez sur la nouvelle branche.

### commit les changements
Apportez des modifications : Modifiez un fichier dans votre projet. Vous pouvez ajouter, supprimer ou modifier du texte, du code, etc. dans le fichier.

Ajoutez et committez vos modifications : Utilisez les commandes suivantes pour ajouter les modifications au suivi de Git et effectuer un commit :
```
git add nom_du_fichier_modifié
git commit -m "Description de votre modification"
```

Remplacez nom_du_fichier_modifié par le nom du fichier que vous avez modifié et ajoutez une description significative pour le commit.

### Push les changements
Une fois les modifications faites, publiez les sur l'environnement a distance.
Si c'est le premier push de la branche. Vous pousserez aussi la nouvelle branche sur l'environnement à distance.
Cette branche sera maintenant disponible a partir de l'environnement à distance

Pousser votre commit sur l'environnement à distance :
```
git push
```

**Mettre a jour votre environnement local lorsqu'il est différent de l'environnement à distance :**
executer cette commande pour récupérer les changements sur l'environnement à distance :
```
git fetch
```

executer cette commande pour appliquer les changements sur l'environnement et les fusionner a votre environnement local :
```
git pull
```
### Changer de branches
Revenez à la branche principale fictive : Si vous souhaitez maintenant fusionner votre nouvelle branche avec la branche principale fictive, utilisez la commande suivante pour revenir à la branche principale :
```
git checkout main_fictif_<ton_nom>
```

### Merge de branches
Fusionnez la nouvelle branche avec la branche active : Utilisez la commande suivante pour fusionner la nouvelle branche avec la branche active :
```
git merge <nom_de_la_branche>
```

Remplacez <nom_de_la_branche> par le nom de la branche que vous avez créée.

Supprimez la branche (si nécessaire) : Si vous n'avez plus besoin de la branche que vous avez créée, vous pouvez la supprimer à l'aide de la commande suivante :

```
git branch -d <nom_de_la_branche>
```

Assurez-vous que vous avez déjà fusionné toutes les modifications nécessaires de cette branche avant de la supprimer.

