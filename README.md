Système de Gestion des Étudiants
Description
Ce projet est une application Spring Boot développée pour gérer une liste d’étudiants en utilisant une base de données MySQL.
L’application expose des services web REST permettant d’effectuer des opérations CRUD (Créer, Lire, Mettre à jour, Supprimer) sur les données des étudiants.

L'objectif principal est de mettre en pratique les concepts de Spring Boot, Spring Data JPA, et REST API.

Fonctionnalités
Ajouter un nouvel étudiant dans la base de données.
Consulter la liste des étudiants.
Modifier les informations d’un étudiant.
Supprimer un étudiant.
Prérequis
Avant de commencer, assurez-vous d’avoir :

Java 8 ou une version supérieure.
Maven 3.x pour la gestion des dépendances.
MySQL comme système de gestion de base de données.
Un IDE compatible avec Spring Boot (par exemple IntelliJ IDEA ou Eclipse).
Structure du Projet
La structure du projet générée via Spring Initializr est organisée comme suit :

php
Copier le code
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── example/
│   │           └── studentmanagement/
│   │               ├── controllers/    # Contient les classes contrôleurs REST
│   │               ├── entities/       # Modèles de données (exemple : Student)
│   │               ├── services/       # Logique métier
│   │               └── repositories/   # Interfaces pour l'accès aux données
│   └── resources/
│       ├── application.properties      # Fichier de configuration
│       └── static/                     # Ressources statiques (si nécessaire)
│       └── templates/                  # Modèles HTML (si applicable)

Configuration de la Base de Données
Ajoutez les paramètres suivants dans le fichier application.properties :

properties
Copier le code
spring.datasource.url=jdbc:mysql://localhost:3306/student_db
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.mvc.pathmatch.matching-strategy=ant-path-matcher
Remarque : Créez une base de données MySQL nommée student_db avant d’exécuter l’application.

Dépendances Principales
Les dépendances suivantes sont incluses dans le fichier pom.xml :

Spring Web : Pour créer et gérer les endpoints REST.
Spring Data JPA : Pour gérer les entités et interagir avec la base de données.
MySQL Driver : Pour connecter l'application à la base de données MySQL.
Spring Boot DevTools : Pour un rechargement automatique lors du développement.
