---
sidebar_position: 1
---

# Maven

## Installation

Site Apache, télécharge le zip du bin
Dézipper les éléments et les enregistrer dans un fichier choisi

Dans les variables d'environnement, dans PATH côté variables utilisateur
Modifier PATH
Ajouter le chemin vers le bin de apache


Pour vérifier l'installation
Ouvrir un invite de commande avec cmd
taper mvn -version

## Créer un nouveau projet Maven

Dans Eclipse : Nouveau Maven Project
Create a simple project
Remplir le groupId (groupe de projets)
Remplir le ArtifactId (nom du projet)
Par défaut la version est à 0.0.1
Par défaut le packaging est un .jar

Dans un invite de commande, se positionner sur le chemin du projet : 
mvn clean install
