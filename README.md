# Presentation of 9/17/2019

* Salle A09/343

  ## Objectif de la présentation: Présenter Git & GitHub via un cas pratique

![](http://www.lalettrem.fr/sites/default/files/logo_societe-generale_4.png)



# Agenda

* Definition VCS: Version Control System
* Présentation Git & GitHub
* Cas pratique

# Table of Contents
* [1)](#Définition VSC: Version Control System)
* [2)](#Git & GitHub)
* [1)](#Cas pratique)
* [1)](#Appendix)

# Définition VSC: Version Control System

* Un **Version Control System**, or **VCS**, permet de tracker l'historique des changements effectués par une ou plusieurs personne(s) affectées à un projet. 
* Le développeur peut, via un VCS, connaitre:
  *  les différents changements
  *  quelle personne a effectué un changement
  * a quel moment le changement a été effectué
  * la raison pour le changement

  
    ![](https://promact.blob.core.windows.net/images/2018/04/Version-Control-System-1024x498.png)



# Git & GitHub

Il existe plusieurs VCS, mais [Git](https://guides.github.com/introduction/git-handbook/) est à la fois  le plus abouti et le plus utilisés par la communauté de développeurs

A vrai dire, selon [Stack Overflow](https://stackoverflow.com/), plus de 85% des développeurs utilisent Git!

![](https://dynalist.io/u/3QWcx08HlnyivJET3XmWvZVf)
[Stack Overflow Developer Survey 2018](https://insights.stackoverflow.com/survey/2018#work-_-version-control)

# Qu'est ce que Git ?
![](https://cdn.vox-cdn.com/thumbor/A4_6e24biy8bp4ahrL-TNfaircI=/0x0:2040x1360/1200x800/filters:focal(1287x538:1613x864)/cdn.vox-cdn.com/uploads/chorus_image/image/63739082/git.0.jpg)

* Git est un programme pour faire du VCS. Il permet de tracker les modifications du ou des codes sources de manière simple. Il a été conçu pour faciliter la coordination entre les programmeurs, et gérer l'historique des codes.
* Git est un outil formidable pour plusieurs raisons: 
  * Avoir le codes au même endroit
  * Avoir un historique des changement
  * Ajouter des informations relatives à chaque changement
  * Savoir la personne qui a fait les modifications
* Git fonctionne principalement avec des lignes de commande.

## Exemple d'utilisation de git

```
git init
git add LICENSE
git commit -m 'initial project version'
```



# Qu'est ce que GitHub?

* [GitHub][https://github.com](https://github.com/) est une plateforme hôte pour le VCS. Il permet à tous les team members de travailler ensemble sur n'importe quel projet, à partir de n'importe quelle machine.
* GitHub permet regrouper et coordonner les différents `git` enregistrés localement
* GitHub permet aussi de faire abstraction de l'ensemble des lignes de commande git. Grâce à [GitHub](GitHub.com) et [GitHub Desktop](https://desktop.github.com/), l'utilisateur peut utiliser l'ensemble du Workflow git sans problème et sans une seule ligne de code. 
  

  ![](https://dynalist.io/u/HbGNi12_fQv5_gpy8pZ3dPDE)



# Cas pratique

Dans le cas suivant, on fait l'hypothèse que nous allons commencer un nouveau projet. Plus précisément, aucun document ou ficher ne se trouve localement et le repository dans GitHub n'existe pas encore.

Nous allons utiliser  [GitHub](GitHub.com) et [GitHub Desktop](https://desktop.github.com/) pour l'ensemble du cas pratique, cela signifie que nous n'allons pas utiliser les lignes de commande. En appendix, vous trouverez l'équivalent Git command-line.

## Step 1: Créer un dossier vide en local

* Ouvrez votre répertoire perso et créez un dossier appelé Repositories 

  

  ![](https://drive.google.com/uc?export=view&id=1vIhNR9q8qvT7pEnUSg4HHWFFoBf5YJbL)

Le repertoire va vous servir à mettre les codes, data, documents etc qui vont vous servir tout le long du projet. Chaque document à l'intérieur de ce dossier va être partagé sur le réseau avec les autres membres de votre équipe.

Il faut savoir que chaque personne de votre équipe va avoir son propre dossier  `Repositories`  dans sa machine. Le dossier `Repositories` va contenir le ou les différents projets en cours. Chaque dossier à l'intérieur de `Repositories` est indépendant des autres dossiers. 

Si une personne de l'équipe a un problème avec son disque dur, cela n'affectera pas le dossier. Ainsi, il n'y a pas de crainte à avoir en cas de perte de donnés. La personne de l'équipe pourra simplement  "cloner" le repository du serveur et retrouver la dernière version. 

## Step 2: Créer un Repository

* Rendez vous sur [https://github.com/] et cliquez sur `New`

  

  ![](https://drive.google.com/uc?export=view&id=123xkU7oLAtYoM0qMJLUOQIRO8Wlf_7Cm)

* Renseignez les champs suivants:
  * Repository name
  * Description
  * Ne cochez pas Initialize this repository with a README
  * Laissez `.gitignore` et `licence` to `None`
  
* Cliquez sur  `Create Repository`

  ![](https://drive.google.com/uc?export=view&id=1aWXFS2-y8RZY_Jxwu7KvttGTQURU9OP3)

  La page qui suit vous indique plusieurs choix a effectuer. Dans la mesure ou nous souhaitons utiliser GitHub Desktop, nous pouvons ignorer les lignes de commande. 


![](https://drive.google.com/uc?export=view&id=1caSZ92v7nCcVuVzwX9SRgN5cIz-TzvoJ)
* Cliquez sur `Set up in Desktop` pour faire la liaison entre GitHub et le dossier en local



## Step 3: Synchroniser Git/GitHub & dossier local

Dans cette étape, nous allons indiquer à GitHub ou cloner  le repository `MyGitHubTest`. Dans cette étape, GitHub va automatiquement créer un dossier caché `.git`. Dès que cette étape est faite, la liaison local ~ GitHub sera établie.

* Vous allez être rediriger vers `x-github-client://openRepo/https://github.com/thomaspernet/MyGitHubTest`


  ![](https://drive.google.com/uc?export=view&id=1fOm7MSPJksmOHePaApaqXjXD5YLcNlG8)

* Après avoir ouvert GitHub Desktop, vous avez la possibilité de cloner le repo

  ![](https://drive.google.com/uc?export=view&id=1E4pV5CtHlmvkxW6RbgLi2dKEyVFqr1Wm)

  

* Veuillez changer le `Local Path` en cliquant sur `Choose` . Dans mon cas le path est
  * `/Users/thomas/Google Drive/Projects/Data_science/GitHub/Repositories` 

  
    ![](https://drive.google.com/uc?export=view&id=1o19hUGopcSyBMys4zu0gakLNj_DfTe4w)
  
* Ensuite, cliquez sur `Clone` pour télécharger le repo MyGitHubTest dans le dossier local repositories 

  ![](https://drive.google.com/uc?export=view&id=1dINOw1RVOHxHbT6gYerU5blSA-ttkc9X)
  

  **Vous êtes all set!**

* Si vous pouvez voir les fichiers cachés, vous devriez apercevoir un nouveau dossier `.git` 


![](https://drive.google.com/uc?export=view&id=1IKsHMmoJeRqvVqKnfgc2j8mIp__baak7)



### GitHub Desktop

Le projet est maintenant synchronisé en local et en remote. Nous pouvons regarder plus en détail l'interface GitHub Desktop. 

![](https://drive.google.com/uc?export=view&id=1i9Q9rwm3KIr7QRvJiZrn_P54KBo8vMBD )



## Step 4: Creation du fichier README

Le fichier `README` permet de décrire le project. C'est le premier élément visible lorsque qu'une personne se rend sur l'URL. Plus le README est détaillé, plus il est facile d'intégrer de nouvelle personne au projet. 

Comme nous n'avons pas utilisé les lignes de commande pour créer un premier `push` , nous devons le faire manuellement. Pour cela, nous allons créer un ficher text et changer l'extension en `.md`. Le fichier va donc être nommé `README.md`
* Ouvrez votre Text Editor favorie. Pour ma part, j'utilise [Typora](https://www.typora.io/)
* Copier/coller le texte suivant 

```markdown
# Description Projet MyGitHubTest

Le projet MyGitHubTest a pour but d'apprendre GitHub
```

* Sauvegarder et renommer le fichier  README.md dans le dossier MyGitHubTest 

![](https://drive.google.com/uc?export=view&id=15JooOmoB_rOYrNeBT5r8z3X7389ejzQT)



Example de `README.md`:

- [Pandas](https://github.com/pandas-dev/pandas)
- [Scikit](https://github.com/scikit-learn/scikit-learn)

## Step 5: Creation du fichier caché .gitignore

Le fichier `.gitignore` va permettre d'indiquer à Git toutes les extensions à ignorer lors de l'étape `add`

* Veuillez ouvrir votre text editor de préférence pour faire de la programmation. Pour ma part, j'utilise [Sublime Text](https://www.sublimetext.com/)

* Copiez/collez le texte suivant 

  ```
  .ipynb_checkpoints
  */.ipynb_checkpoints/*
  *.gz
  *.csv
  *.png
  *.pdf
  ```

  

* Sauvegardez et renommer le fichier  `.gitignore` dans le dossier `MyGitHubTest`


  ![](https://drive.google.com/uc?export=view&id=1rt0CwZO5OM-1TijfuoD9rP7Bou6toYJt)



## Step 6: Synchroniser les changements avec Git/Github

Pour synchroniser un changement local vers Git puis Github, il faut suivre une procédure en 3 temps:

* `Add`: Indiquer à Git le ou les fichiers a synchroniser
* `Commit`: Indiquer à Git le motif du/des changements
* `Push`: Envoyer le changement vers le serveur en remote (ie GitHub)

### Add to Stage

La première étape consiste a ajouter le/les fichiers dans le stage

* Ouvrez GitHub Desktop. Si vous êtes dans le bon repository, vous devriez voir deux nouveaux fichiers à gauche de l'écran:
  * `README.md`
  * `.gitignore` 
  * La partie en vert indique les changements
  * La partie en rouge indique les suppressions.

    ![](https://drive.google.com/uc?export=view&id=1u6qeiLuDFB2-FIOFO63o7mrn0FAXNZAJ)



### Commit 

La seconde étape sert expliquer les changements effectués. 

* Cliquez sur la bande `Summary (required)`
  * A noter que si la partie `change` a seulement un fichier, GitHub Desktop va automatiquement indiquer le commit avec update + nom du fichier 
  * Dans notre cas, nous pouvons noter initialisation project 
* Ensuite, cliquer sur `commit`

![](https://drive.google.com/uc?export=view&id=1nNnpxT3mHcJ7kMeHtUygMzHM9nPPLtMN)



### Push to Remote

La dernière étape consiste a envoyer les changements dans le serveur remote (i.e. GitHub). Git va se charger de faire la mise à jour du dossier automatiquement. 

GitHub indique de publier d'abord la branche `master`. Lors des prochains `push`, le message va disparaitre. Il y a le message car nous avons initialiser le projet via GitHub desktop.

![](https://drive.google.com/uc?export=view&id=16nFNxG_dnl4k9EldVYtNq0WrMGk3jZQb)

Voilà! GitHub et le dossier local sont maintenant a jour. 

![](https://drive.google.com/uc?export=view&id=1qNVMpNUJ6DnKROgJnJa5PQ5qQgtCaNvj)

Veuillez vous rendre sur le lien [Github](https://github.com/thomaspernet/MyGitHubTest) pour voir le changement.

![](https://drive.google.com/uc?export=view&id=1r1CBpp1_FODbH6_Rp8XRsy6cl_seHIo4)

# Workflow project

La branche `master` doit rester une branche de déploiement, c'est à dire quelle ne doit pas servir à faire des tests. Pour cela, il faut créer une ou des branches à part entière(s) de la branche `master`. Des que la phase de test est finie, il suffit de faire un merge entre les deux branches.

Dans l'exemple suivant, nous allons créer un fichier python dans la branche  `master`. Le fichier python va nous servir de socle pour le développement du projet. Afin de ne pas créer de bug entre les utilisateurs du répo, nous allons créer une branche de développement, appelée `branchDev`. Dès que le développement est fini, nous allons merger les deux branches pour rendre utilisable la branche `master`. 

## Step 1: Creation fichier python
Dans un premier temps, nous allons créer un fichier python avec les lignes de code suivantes:

```python
import pandas as pd
import numpy as np
### Step 1, create an empty array
np.random.rand(3,3)
#### below development steps
```



* Ouvrez votre Text editor favori, pour ma part j'utilise [Atom](https://atom.io/), avec le package [hydrogen](https://atom.io/packages/hydrogen)
* Copiez/collez le code ci-dessus et enregistrez le fichier intitulé myFirstPython.py  dans le repertoire `MyGitHubTest`

![](https://drive.google.com/uc?export=view&id=1QbiznE2FzhNL7NSzzxX_EducJAifAJSM)

Des que le fichier python est enregistré, veuillez faire les trois étapes nécessaires pour envoyer les changements dans Git/GitHub

![](https://drive.google.com/uc?export=view&id=1rpyFPGqh0cciHjNHKzDlC6WdwB1ffWwB)

## Step 2: Création d'une branche

La création d'une branche va dupliquer la branche master selon le dernier commit. Cela va permettre de retrouver à l'identique les fichiers de la branche `master`, disponible dans la nouvelle branche nommée `brancDev` . Chaque modification dans la branche `branchDev`  n'affectera pas la branche master . 

Par exemple, il a été décidé d'ajouter une nouvelle feature au code `myFirstPython.py`. Pour éviter de créer des bugs dans la branche `master` (i.e éviter que les nouveaux utilisateurs clonant le repo se retrouve avec un programme ne fonctionnant pas), nous allons ajouter cette nouvelle feature dans une branche. 

* Ouvrez GitHub Desktop, puis localisez l'onglet Current branch 

  ![](https://drive.google.com/uc?export=view&id=1TcfGAfsE1J2K5R9SdEvDDihiojpVCOn8)

* Après avoir cliqué sur l'onglet, vous devriez apercevoir la branche master qui est la branche par default. Elle doit toujours le rester!

* Cliquez sur `Filter` et rentrez `branchDev`

* Finalement, créez la branche en cliquant sur `Create new branch`


  ![](https://drive.google.com/uc?export=view&id=1zG0LW1qnbEvQJMUrgmC6nEwRx4GSHMAw)

  

* GitHub vous demande confirmation, cliquez sur `Create branch`

![](https://drive.google.com/uc?export=view&id=1Vb42Zqt1YosavL9i4l3wsMl8kRIl5HWj)
* Pour indiquer à GitHub la création d'une nouvelle branche, vous devez cliquer sur `Publish branch`
* Vous devriez noter que GitHub Desktop a changé la branche. La nouvelle branche de travail est devenue `branchDev`

![](https://drive.google.com/uc?export=view&id=1hXOGVrHfMBtSQ-XqXo_ipapXS4IOHd7B)

Rendez vous sur thomaspernet/MyGitHubTest pour visualiser la création de la nouvelle branche. 

## Step 3: Ajouter une feature

Maintenant que la branche est ouverte, nous pouvons apporter une modification au code. Pour cela, ouvrez le fichier myFirstPython.py  et collez les lignes de code suivantes:

```python
##### Create 2 random arrays
x = 4 * np.random.rand(100)
mu, sigma = 0, 1
y =  2 + 3 * x +  np.random.normal(mu, sigma, 100)

import matplotlib.pyplot as plt

plt.scatter(x, y, alpha=0.5)
plt.title('Scatter plot pythonspot.com')
plt.xlabel('x')
plt.ylabel('y')
plt.show()
```



Les codes est très simple. Il construit deux arrays selon la fonction: $y = 2 + 3x + e$
* x = 4 * random noise
* y = 2 +  3 * x +  error term 

Ensuite, il construit un scatterplot avec x & y

![](https://drive.google.com/uc?export=view&id=1ZWYjY80llasYQuEWAdH_BqPz94UjYblZ)

* Pour ajouter les changements sur GitHub, il suffit de faire les 3 opérations (add, commit, push)
  * Faites attention a bien faire le commit dans la branche `branchDev`

Pour vous rendre compte de la différence, allez dans le site GitHub, sélectionnez la [branche](https://github.com/thomaspernet/MyGitHubTest/blob/master/myFirstPython.py)  ` master`, et ouvrez le fichier  `myFirstPython.py`. Renouvelez l'opération mais pour la [branche](https://github.com/thomaspernet/MyGitHubTest/blob/branchDev/myFirstPython.py) `brandDev`

### Branche Master

![](https://drive.google.com/uc?export=view&id=1rRp5C5w8PrjwM1Pmr12RioFns1HKAgD0)

### Branche branchDev

![](https://drive.google.com/uc?export=view&id=1l08uKyKVVo_MfQcZvML66yncGEhLBlTZ)

## Step 4: Ouvrir un Pull request

* La fonction `Pull Request` est au coeur de la collaboration sur GitHub. Lorsqu'une personne de l'équipe ouvre un ` pull request`, elle propose de faire un changement ou demande à une autre personne de vérifier le code.
* Un `pull request`est un genre de discussion entre les différentes parties du projet
*  Des que le Pull Request est validé, c'est à dire que l'objectif de la branche a été atteint, une personne de l'équipe peut proposer de faire un merge avec la branche master . Lors d'un `Pull Request`, il est possible de voir les différences entre le code d'origine et les modifications. 
* Pour contacter directement une personne de la team, l'utilisateur peut utiliser "@" suivit du nom. 

Nous allons effectuer un `pull request` pour la branche `branchDev`. Une personne de la team trouve interessant d'intégrer le calcul de la pente et de l'intercept dans le programme. Il peut suggérer un ajout via un `pull request.
* Dans GitHub Desktop, rendez-vous dans la branche `branchDev` et cliquez sur `Create Pull Request

  ![](https://drive.google.com/uc?export=view&id=1av0XYwPnqyvktMakedcYBk8qJ4Za3Cwe)

* Vous allez être automatiquement redirigé vers GitHub Website 
  
  * https://github.com/thomaspernet/MyGitHubTest/compare/branchDev
  
* Vous avez maintenant la possibilité d'ajouter un commentaire par rapport au dernier commit effectué dans la branche `branchDev` et le commit n -1 effectué dans master 

  ![](https://drive.google.com/uc?export=view&id=1eMG7Rq2gNVeesONPVKZNBZjPs6Se3G6f)

* En descendant un peu vers le bas de la page, vous pouvez voir la différence entre le commit n-1 et le commit n

  ![](https://drive.google.com/uc?export=view&id=1pvGUQ5m99olHmF4xcWpYZEhWW4ArFn35)

* Dans notre example, nous pouvons ajouter un nouveau commentaire indiquant notre interêt de voir le calcule de la slope et de l'intercept
  
```
It would be great if we can print the slope and intercept in the program
  ```
  
  
  
  ![](https://drive.google.com/uc?export=view&id=13Vo6tuwFzPJ4v8CoFsTMCU22vJIUE0Lj)
  
* Le fil de la discussion est disponible via ce [lien](https://github.com/thomaspernet/MyGitHubTest/pull/1)

  ![](https://drive.google.com/uc?export=view&id=1kFUKZpt7j18RV_tkA_P5nr5O_vWJgZ4r)

* Nous pouvons ajouter cette nouvelle demande dans le code. Ouvrez le fichier `myFirstPython.py`  et collez le code suivant:
```python
from scipy import stats
### Compute the linear relationship
slope, intercept, r_value, p_value, std_err = stats.linregress(x,y)
print("The slope is {0:.2f} and the intercept is {1:.2f}".format(slope,
 intercept))
```



* Normalement, on devrait trouver un intercept proche de 2 et une slope proche de 3. La difference vient du terme d'erreur.

  ![](https://drive.google.com/uc?export=view&id=1AFX9HiY9dVvD5PaGY1GhHKWYfWb-UQdp)
* Comme d'habitude, envoyez les changements avec la routine: add, commit, push 

## Step 5: Merger la Pull Request

Tout d'abord, nous pouvons notifier à la personne de l'équipe ayant demandé la feature que cette dernière à bien été ajoutée. Pour cela on peut utiliser le "@" + nom. Comme la requête a été exécuté sans problème, le propriétaire du projet peut fermer et commenter la branche. En cliquant sur Close and comment , cela va fermer le `pull request`

![](https://drive.google.com/uc?export=view&id=1DvcV5CfP4iBuwqA23qcuZp0UshhzUth2)

Comme la discussion est fermée et les requêtes ajoutées, nous pouvons faire le merge entre la branche `branchDev`  et la branche  `master`.
* Ouvrez GitHub Desktop, et choisissez la branche master 
* cliquez sur `choose a branch to merge into master `

![](https://drive.google.com/uc?export=view&id=1hlPuup8e4qlgKChzWqTnGGBltLemFjBd)
* Ensuite, il faut choisir la branche `branchDev` puis confirmer

  ![](https://drive.google.com/uc?export=view&id=1I_nFzORRl1xErL5eDshNrmeU1-c-BtwM)
* Si le merge est un succès, GitHub Desktop propose de faire le push

  ![](https://drive.google.com/uc?export=view&id=1SoLsqr4FQAW0euh5oJQX1QxQawvwUBS6)

Pour vous rendre compte de la manipulation réalisée par GitHub, il faut se rendre sur le site [GitHub](https://github.com/thomaspernet/MyGitHubTest/tree/master) du répo et ouvrir le fichier `myFirstPython.py`. Le fichier python se trouve dans cet URL. 

Le fichier python a bien été mis à jour

![](https://drive.google.com/uc?export=view&id=1_HbzUfh-w-MklFKvPVH0m9gZc5-TaCO1)

Pour découvrir les differences entre les deux fichiers, il faut cliquer sur `History`, ou sur ce [lien](https://github.com/thomaspernet/MyGitHubTest/commit/d87d56e24f4cfe35b663ff18241af9bea46cf6a3#diff-6b34238823334484390a1b97cd13b297).

![](https://drive.google.com/uc?export=view&id=1LRKB709SPlKabsI779e8oCrN3tQqdZ2T)

## Step 6: Supprimer la branche branchDev
Maintenant que le développement de cette branche est fini, il est possible de supprimer la branche `branchDev`

* Dans GitHub Desktop, rendez vous dans la branche `branchDev` puis dans le ruban, sélectionnez `delete`
  ![](https://drive.google.com/uc?export=view&id=1VOFvFDds8UWwwvkDqTt9KDW3Z5gZWtE-)

* Dans la fenêtre qui va s'afficher, cochez `Yes, delete this branch on the remote`

  ![](https://drive.google.com/uc?export=view&id=1v8ctxpiSjD-9cU6oxBhSKYaecUP38ptG)
* Attendez quelques instants. La branche devrait être supprimer automatiquement. 

Si vous vous rendez dans le site GitHub du répo, vous pouvez constater qu'il ne reste plus que la branche `master`

![](https://drive.google.com/uc?export=view&id=1ZKSZAX_FyOY_kkPuRA2-j0uJ8mZpuDTr)

# Appendix

Voici l'équivalent du workflow avec la ligne de commande. A noter qu'il n'est pas possible de faire un `pull request` en ligne de commande. Cette feature est spécifique à GitHub.

## Step 1: Créer un Repo
Allez sur [Github](https://github.com/thomaspernet), et créez un repo appelé `MyGitHubTest_CommandLine`

* Description:
  * A second repository to test Git & GitHub with command line only 
Ne fermez pas la page

## Step 2: Créer un dossier en local

Maintenant que le répo est créé en remote, il faut le créer en local et ajouter `git`  et la connection en remote. 

* Choisissez un dossier dans lequel vous souhaitez créer le répo `MyGitHubTest_CommandLine`
* Pour ma part, le nouveau dossier va être créé dans `/Users/thomas/Google Drive/Projects/Data_science/GitHub/Repositories/` 
  * Pour créer un nouveau dossier avec la ligne de commande: `mkdir`
  
  ```shell
  mkdir '/Users/thomas/Google Drive/Projects/Data_science/GitHub/Repositories/MyGitHubTest_CommandLine' 
    Step 3: Etablir la connection 
    Avant de créer le répo en local et la connection GitHub, il est préférable d'ajouter des fichiers. Tout d'abord, ajoutons un README.md
    ```
  
    

Le plus simple est d'utiliser la commande  `echo` 

```shell
echo "# MyGitHubTest_CommandLine" >> README.md
```



La commande ci dessus va simplement créer un fichier appelé `README.md`  et ajouter en en-tête `# MyGitHubTest_CommandLine`

Maintenant, il faut initialiser le répo git . La commande ci-dessous va simplement créer un dossier caché `.git`. C 'est la même étape que lors du clone en section **Step 3: Synchroniser Git/GitHub & dossier local**

```shell
git init
```



Les prochaines étapes sont assez simples, il suffit d'ajouter le `README.md`  dans Git et l'envoyer dans la remote

1)  Ajouter à Git

```shell
git add README.md
git commit -m "first commit"
```



2) Connecter Git & la remote 

```shell
git remote add origin https://github.com/thomaspernet/MyGitHubTest_CommandLine.git
```



3) Synch avec la remote

```shell
git push -u origin master
```



Si vous allez sur [thomaspernet/MyGitHubTest_CommandLine](https://github.com/thomaspernet/MyGitHubTest_CommandLine) et rafraîchissez la page, vous devriez voir le `README.md`

## Step 4: Ajouter le .gitignore

Comme avec GitHub desktop, il est préférable de créer un `.gitignore` . C'est très similaire à l'étape d'avant. 

Comme nous faisons toute la démo en ligne de commande, on peut utiliser l'éditeur vim pour créer et ajouter du contenu. 

```shell
vim .gitignore
```



Ensuite, collez le texte suivant:

```shell
.ipynb_checkpoints
*/.ipynb_checkpoints/*
*.gz
*.csv
*.png
*.pdf
```



Pour quitter vim, appuyez sur `esc` et `:wq!` . 

Puis envoyez vers GitHub

```shell
git add .gitignore
git commit -m "fixing .gitignore"
git push -u origin master  
```



## Step 5: Création fichier python

Avant de passez dans la branche de développement, il faut créer un fichier python. 

```shell
vim test.py
```

puis

```python
import pandas as pd
import numpy as np
### Step 1, create an empty array

np.random.rand(3,3)

#### below development steps
```

Ensuite, synch avec GitHub

```shell
git add test.py
git commit -m "Add python file"
git push -u origin master
```



## Step 6: Création branche

Pour créer une branche, il suffit d'utiliser l'argument branch . On va appeler la nouvelle branche `branchDev`

```shell
git branch branchDev
```



Pour connaitre le nom des branches disponibles dans le répo:

```shell
git branch
```



maintenant que la branche est disponible en local, il faut synch avec GitHub: `git push <remote> <branch>`

```shell
git push https://github.com/thomaspernet/MyGitHubTest_CommandLine branchDev
```



## Step 7: Modifier le fichier python

La branche développement a été créé. Nous pouvons des à présent modifier le fichier python dans la branche. Pour cela, il faut changer de branche. L'argument `checkout` permet de naviguer entre les branches avant de faire un commit. Attention, si vous changez de branche, vous trouverez le contenu des fichiers de cette branche. Plus précisément, si vous faites un changement dans le fichier `test.py`  dans la branche `branchDev`  alors le fichier `test.py` n'aura pas le même contenu si vous switchez vers la branche `master`

```shell
git checkout branchDev
```



On va pouvoir modifier le fichier python. Via la ligne de commande, on utilise vim puis on clique sur ` i` pour insérer du contenu

```shell
vim  test.py
```



et on ajoute:

```python
##### Create 2 random arrays

x = 4 * np.random.rand(100)
mu, sigma = 0, 1
y =  2 + 3 * x +  np.random.normal(mu, sigma, 100)

import matplotlib.pyplot as plt

plt.scatter(x, y, alpha=0.5)
plt.title('Scatter plot pythonspot.com')
plt.xlabel('x')
plt.ylabel('y')
plt.show()
```



Pour quitter l'éditeur, `esc`  et `:wq!` 

On envoie sur GitHub

```shell
git add test.py
git commit -m "Change stuff"
git push -u origin branchDev
```

## Step 8: Merge avec Master

Maintenant que le fichier `test.py`  est fini, nous allons pouvoir merger avec `master` 

Attention a bien changer de branche.

```shell
git checkout master
git merge branchDev
```

Finalement, on envoie vers GitHub

```shell
git add test.py
git commit -m "Merge stuff"
git push -u origin master
```



## Step 9: Supprimer la branche

La dernière étape consiste à  supprimer la branche  `branchDev`. C'est très simple. Il faut faire cela en deux temps:

Tout d'abord, on supprime la branche de la remote:

### Clean Remote
```shell
git push https://github.com/thomaspernet/MyGitHubTest_CommandLine --delete branchDev
```

Ensuite, on clean le repo en local

```shell
git branch -d branchDev
```



## Appendix



| Task                                                         | Code Syntaxe                                   | Code                                                         | Image                                                        |
| ------------------------------------------------------------ | ---------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Create README                                                | echo                                           | echo                                                         | ![](https://drive.google.com/uc?export=view&id=15JooOmoB_rOYrNeBT5r8z3X7389ejzQT) |
| Initialize git repo                                          | git init                                       | git init                                                     | ![](https://drive.google.com/uc?export=view&id=1E4pV5CtHlmvkxW6RbgLi2dKEyVFqr1Wm) |
| Step 1: Add file to stage                                    | git add FILENAME.EXTENSION                     | git add README.md                                            | ![](https://drive.google.com/uc?export=view&id=1u6qeiLuDFB2-FIOFO63o7mrn0FAXNZAJ) |
| Step 2: Add commit and description                           | git commit -m "DESCRIBE COMMIT"                | git commit -m "first commit"                                 | ![](https://drive.google.com/uc?export=view&id=1nNnpxT3mHcJ7kMeHtUygMzHM9nPPLtMN) |
| Step 3: Push to GitHub. If first time, connect local to remote | git remote add origin                          | git remote add origin https://github.com/thomaspernet/MyGitHubTest_CommandLine.git | ![](https://drive.google.com/uc?export=view&id=16nFNxG_dnl4k9EldVYtNq0WrMGk3jZQb) |
| Step 3: Push to GitHub. If connection local to remote already exists | git push -u origin                             | git push -u origin master                                    | ![](https://drive.google.com/uc?export=view&id=16nFNxG_dnl4k9EldVYtNq0WrMGk3jZQb) |
| Create branch                                                | git branch NAME BRANCH                         | git branch branchDev                                         | ![](https://drive.google.com/uc?export=view&id=1TcfGAfsE1J2K5R9SdEvDDihiojpVCOn8) |
| Add branch to GitHub                                         | git push                                       | git push https://github.com/thomaspernet/MyGitHubTest_CommandLine branchDev | ![](https://drive.google.com/uc?export=view&id=1hXOGVrHfMBtSQ-XqXo_ipapXS4IOHd7B) |
| Switch branch:                                               | git checkout NAME BRANCH                       | git checkout branchDev                                       | ![](https://drive.google.com/uc?export=view&id=1hlPuup8e4qlgKChzWqTnGGBltLemFjBd) |
| Merge branch with master                                     | git merge NAME BRANCH                          | git merge branchDev                                          | ![](https://drive.google.com/uc?export=view&id=1I_nFzORRl1xErL5eDshNrmeU1-c-BtwM) |
| Delete branche: 1) In Github                                 | git pushgit push <REMOTE> --delete BRANCH NAME | https://github.com/thomaspernet/MyGitHubTest_CommandLine --delete branchDev | ![](https://drive.google.com/uc?export=view&id=1VOFvFDds8UWwwvkDqTt9KDW3Z5gZWtE-) |
| Delete branche: 1) In Git                                    | git branch -d BRANCH NAME                      | git branch -d branchDev                                      | ![](https://drive.google.com/uc?export=view&id=1v8ctxpiSjD-9cU6oxBhSKYaecUP38ptG) |
|                                                              |                                                |                                                              |                                                              |
