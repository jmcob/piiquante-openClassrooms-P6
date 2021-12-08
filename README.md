# piiquante - openClassrooms web developer P6 2021

/!\ Le projet n'est pas utilisable pour l'utilisateur que vous êtes, je vous suggère de me contacter a partir de mon site web www.jmax.dev

## Introduction

Après un cours openClassrooms de Will Alexander, nous sommes propulsés dans le backend JS avec node.js;
Nous installons tous les modules nécéssaires au backend dans ce repo :

1. node.js tout d'abord pour initialiser le repo;

2. git, installation du repo sur github;

3. express et mongoose pour mongoDB;

4. helmet, dotenv, multer;

## Dotenv

Dotenv permet de travailler avec des variables d'environnement et sécuriser les mots de passe d'un backend node.js.

La documentation de dotenv se trouve ici : https://www.npmjs.com/package/dotenv (en anglais).

Succintement, il vous faudra installer dotenv sur le projet, puis definir une constante qui vaudra [require('dotenv').config()] dans le fichier app.js. Un fichier nommé tout simplement [.env] sans les crochets stockera les données sensibles qui ne peuvent pas être partagées publiquement sur GitHub par exemple. Vous avez un exemple de ces données sur .env.example dans ce projet.

Ce fichier pourra tout de même etre envoyé sur les serveurs d'hébergement de manière sécurisée, comme Heroku ou Google Workspace.

## Multer

Multer récupère et stocke sur le serveur les fichiers envoyés par les utilisateurs. Ici, il est configuré de manière à stocker dans le dossier images/ les images de sauces proposées par chaque utilisateur.

## piiquante est un site d'avis gastronomiques

Nous pouvons ici poster des sauces : une route sauce est ajoutée avec un controller (un middleware);

Nous pouvons aussi y mettre des likes ou des dislikes;

Le site web est authentifiée par utilisateur et mot de passe (route auth);


## Node.js

Nous utilisons ici node.js pour construire le backend et ainsi ajouter les modules nécéssaires déja cités.

pour lancer ce programme, vous devez disposer du frontend openclassrooms disponible sur https://github.com/OpenClassrooms-Student-Center/Web-Developer-P6

Sur un terminal dans le dossier du frontend, lancez "ng serve"

Dans le dossier de ce backend, dans un terminal lancez "nodemon server"


## Express()

Nous utilisons express() pour la configuration du router. Express est un module de node.js et un framework JS. Express permet d'appliquer le CRUD à notre application.


## Mongoose

Mongoose facilite la communication avec une base de donnée mongoDB ; mongoose est conçu pour node.js dont il est un module. Créer un schéma, appliquer le CRUD avec notre base de donnée, tout est possible avec Mongoose.
Utilisation de dotenv pour securiser l'acces a mongoDB.

## Helmet

Helmet permet a l'application de respecter les recommandations OWASP.

