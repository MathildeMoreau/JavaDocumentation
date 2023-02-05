---
sidebar_position: 2
---
# Les controllers

## Associer un controller à une vue Thymeleaf

Dans pom.xml

Importer la dépendance spring-boot-starter-thymeleaf

Créer un package Controller et créer le controller
Au dessus de la classe : annotation @Controller

Créer le chemin :
Annotation GetMapping(value="chemin")
Créer une String fonction qui prend en paramètre un Model (springframework.ui.model)
et qui retourne : return "nomPage"


Dans resources : 
Créer un dossier templates
Créer le fichier nomPage.html


Relancer le serveur et aller sur le chemin :)

