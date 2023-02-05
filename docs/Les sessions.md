---
sidebar_position: 3
---

# Les sessions

Permet de garder des informations en mémoire le long de la session utilisateur.

## Côté servlet

Déclarer un élément : HttpSession session = request.getSession();

Récupérer les paramètres :
String nom = request.getParameter("nom");

Les envoyer à la session : 
session.setAttribute("nom", nomElement);

## Côté JSP 

Dans un if , tester si : !empty sessionScope.nom

Et afficher ${sessionScope.nom}