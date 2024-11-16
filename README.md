# Projet Spring Boot - Gestion des Étudiants

## Description
Ce projet est une application de gestion des étudiants développée avec Spring Boot. Elle expose une API REST permettant de créer, lire, mettre à jour et supprimer des informations sur les étudiants, ainsi que de réaliser des opérations supplémentaires comme compter les étudiants ou regrouper par année de naissance.

---

## Fonctionnalités
- Ajouter un nouvel étudiant
- Supprimer un étudiant par ID
- Lister tous les étudiants
- Compter le nombre total d'étudiants
- Regrouper les étudiants par année de naissance

---

## Prérequis
Avant de commencer,on doit installé les outils suivants :
- [Java JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) (version 11 ou supérieure)
- [Maven](https://maven.apache.org/)
- [MySQL](https://www.mysql.com/) (ou une autre base de données compatible)
- [Postman](https://www.postman.com/) (pour tester l'API)
- Un IDE (IntelliJ IDEA, Eclipse, ou autre)

---

src
├── main
│   ├── java
│   │   ├── com.example.demo
│   │   │   ├── controllers    # Contrôleurs REST
│   │   │   ├── entities       # Entités JPA
│   │   │   ├── services       # Services métier
│   │   │   └── repositories   # Repositories Spring Data JPA
│   ├── resources
│       ├── application.properties  # Configuration de l'application



