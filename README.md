# Formation-Structure-Projet-Python-Django
Donner les étapes de création d'un projet Django

Bonjour, ce fichier vous donnera les différentes étapes de création d'un projet Django; Alors sans plus tarder, nous allons énumérer ces différentes étapes.

Avant de commencer toute création, il faut dans un premier temps installer notre IDE, soit VSCODE ou PYCHARM ( posibilité de prendre l'environnement que vous preférez).
Pour la suite de mon explication, j'utilise VSCODE.

ETAPE 1: CREATION DU REPERTOIRE 

Cette étape consiste à créer un dossier qui contiendra notre projet (exemple: ATOS2024).

ETAPE 2: LA CREATION DE L'ENVIRONNEMENT VIRTUEL

Une fois dans le dossier on peut l'ouvrir avec le terminal et saisir "code ." dans le terminal qui pointe dans le dossier, une fois cela fait, il va lancer l'ouverture dans Vscode.
Une fois dans notre environnement vscode, il nous faut ouvrir le terminal et passer à la création de notre environnement virtuel.
Pour mon cas je travail sur windows alors ..

1-Installer python 
2-vérifiez si pip est parfaitement installé 
3-Création de l'environnement virtuel avec la commande : python -m venv venv (le deuxième venv peut être remplacé par le nom que l'on souhaite utiliser pour son environnement)
4-Activation de l'environnement avec la commande : venv\Scripts\activate 
une fois cette commande validé, nous nous retrouverons directement dans notre environnement virtuel (venv).

ETAPE 3: INSTALLATION DE DJANGO 

une fois dans le venv, il faut installer d'abord django avant tout autre chose. Alors pour le faire on utilise la commande : 
-pip install django 

ETAPE 4: CREATION DU PROJET DJANGO 

Après installation de django, nous pouvons maintenant passer à la création de notre projet django; Nous entrons maintenant la commande suivante : 
- django-admin startproject nom_du_projet

ETAPE 5: CREATION D'UNE APPLCATION 

pour la créationde l'application, il nous suffit de taper la commande:

django-admin startapp nom_application

ETAPE 6: LA CONFIGURATION DE NOTRE PROJET ET APPLICATION 

1- le setting.py 

le setting nous permet de configurer la connexion à la base de données, la route vers les templates, les fichiers static et bien d'autres élements qu'on veut pour notre projet. 
ajouter l'application crée dans la liste de nos applications dans INSTALLED_APPS = [  ]

configurer la routes vers les templates dans TEMPLATES = [ ]

on peut gérer les autres configs du projet à l'intérieur du fichier.

2-le fichier urls.py  

il nous permet de gérer les routes de nos applications 

urlpatterns = [ path('admin/', admin.site.urls)] apres les importations des urls de chaque application.


3-Création du dossier templates 

Ce dossier templates nous permettra de gérer les templates de chaque application dans un dossier portant le nom de l'application pour éviter les conflits de routes à la suite. 






