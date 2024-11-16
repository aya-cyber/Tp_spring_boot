**Système de Gestion des Étudiants**
Ce projet est une application web développée avec Spring Boot, permettant de gérer une liste d’étudiants. Il expose des services REST pour effectuer des opérations CRUD (Créer, Lire, Mettre à jour, Supprimer) sur les données des étudiants.

L’objectif principal est de mettre en pratique les concepts de Spring Boot, Spring Data JPA, et REST API.

**Fonctionnalités**
Gestion des Étudiants :
Ajouter un nouvel étudiant.
Consulter la liste des étudiants.
Modifier les informations d’un étudiant.
Supprimer un étudiant.

**Prérequis**
Java 8 ou supérieur.
Maven 3.x pour la gestion des dépendances.
Un IDE compatible avec Spring Boot (par exemple, IntelliJ IDEA ou Eclipse).
MySQL comme système de gestion de base de données.
Structure du Projet
La structure du projet générée via Spring Initializr est organisée comme suit :

controllers : Contient les classes contrôleurs REST gérant les requêtes HTTP.
entities : Contient les classes entités représentant les modèles de données (par exemple, Student).
services : Contient la logique métier pour gérer les étudiants.
repositories : Contient les interfaces pour l'accès aux données via JPA.

**Configuration de la Base de Données**
Ajoutez les paramètres suivants dans le fichier application.properties :

spring.datasource.url=jdbc:mysql://localhost:3306/student_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.mvc.pathmatch.matching-strategy=ant-path-matcher

**Technologies Utilisées**
Spring Boot : Framework pour la création de l'application.
Spring Data JPA : Pour l'accès aux données et l’interaction avec la base de données.
MySQL : Système de gestion de base de données.
Spring Boot DevTools : Pour un rechargement automatique lors du développement.

Voici les principales dépendances utilisées dans le projet :

Spring Web : Pour gérer les endpoints REST.
Spring Data JPA : Pour la gestion des entités et des opérations CRUD.
MySQL Driver : Pour connecter l'application à la base de données MySQL.
Spring Boot DevTools : Pour faciliter le développement.
