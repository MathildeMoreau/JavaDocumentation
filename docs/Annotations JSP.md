---
sidebar_position: 2
---

# Les annotations

Test de texte.

## @WebServlet

-> "import jakarta.servlet.annotation.WebServlet;"

@WebServlet
    Paramètres : name = "" , urlPatterns = {"", ""}


## Associer une servlet à une vue

 Au dessus de la classe, utiliser une annotation pour indiquer l'URL à suivre : 
 @WebServlet("/testaffichage")


 Dans méthode doGet() : 
 this.getServletContext().getRequestDispatcher("/WEB-INF/nomFichier.jsp").forward(request, response);