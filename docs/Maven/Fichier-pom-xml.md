---
sidebar_position: 3
---
# Fichier pom.xml

Le fichier est découpé en plusieurs parties : 
- En tête : contient la définition du pom, version du projet et les informations éventuelles sur le parent
- Les dépendances : entre balises < dependencies>
- Le build : Entre balises < build>

## Déclarer les propriétés

    <properties>
        <maven.compiler.source>1.8</maven.compiler.source>
        <maven.compiler.target>1.8</maven.compiler.target>
    </properties>

## Déclarer une dépendance

"< dependencies>
    < dependency>
        < groupId>group < /groupId>
        < artefactId>artefact< /artefactId>
        < version>version< /version>
    < /dependency>
< /dependencies>"

## Ajouter une dépendance existante 

<ul>
    <li>Aller sur le site : https://mvnrepository.com/</li>
    <li>Rechercher la dépendance souhaitée</li>
    <li>Cliquer sur la version de la dépendance souhaitée</li>
    <li>Copier / coller le code Maven</li>  
</ul>

Dans la console : 
mvn clean install

## Ajouter un plugin
Dans la balise < build >
<ul>
    <li>Insérer balise parente plugins </li>
</ul>


## Heritage entre fichiers pom

Il est possible d'avoir des fichiers parents ou enfants.

Si le fichier est enfant : 
<ul>
    <li>On déclare une balise parent</li>
    <li>La balise reprend l'artifactID, le groupId et la version du parent</li>
</ul>

Si le fichier est parent : 
<ul>
    <li>On déclare une balise modules</li>
    <li>On insère une balise module pour chaque enfant</li>
</ul>

Attention l'ordre des balises module est importante !