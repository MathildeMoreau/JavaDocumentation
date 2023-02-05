---
sidebar_position: 1
---

# JSP Java Server Pages

Test de texte.

## Créer une servlet

Dans Src / main / Créer un package

Clic droit -> new Servlet

## Associer une servlet à une vue

 Au dessus de la classe, utiliser une annotation pour indiquer l'URL à suivre : 
 @WebServlet("/testaffichage")


 Dans méthode doGet() : 
 this.getServletContext().getRequestDispatcher("/WEB-INF/nomFichier.jsp").forward(request, response);