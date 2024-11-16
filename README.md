# Projet Spring Boot : Gestion des Étudiants

## Description
Ce projet est une application RESTful développée avec Spring Boot pour gérer les étudiants. Elle propose des fonctionnalités telles que la création, la suppression, la récupération, et le comptage des étudiants. Les données sont persistées dans une base de données MySQL.

---

## Fonctionnalités
- **Ajout d'un étudiant** : Enregistrement des informations d'un étudiant (nom, prénom, date de naissance).
- **Suppression d'un étudiant** : Suppression d'un étudiant par son ID.
- **Récupération des étudiants** : Liste de tous les étudiants.
- **Comptage des étudiants** : Nombre total d'étudiants enregistrés.
- **Nombre d'étudiants par année de naissance** : Statistiques regroupées par année de naissance.

---

## Prérequis
- Java 17 ou supérieur.
- MySQL installé et configuré.
- Maven 3.8 ou supérieur.
- Outil de développement (IntelliJ).

---

## Installation
1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/hafsaazizi/gestion-etudiants.git
   ```
2. Configurez la base de données MySQL :
   - Créez une base de données nommée `studentdatabase`.
   - Mettez à jour le fichier `application.properties` si nécessaire :
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/studentdatabase?serverTimezone=UTC
     spring.datasource.username=VotreNomUtilisateur
     spring.datasource.password=VotreMotDePasse
     ```
3. Installez les dépendances et lancez l'application :
   ```bash
   mvn spring-boot:run
   ```

---

## Points de Terminaison de l'API
### Base URL : `http://localhost:8080/api`
| Méthode | URL                  | Description                              |
|---------|----------------------|------------------------------------------|
| GET     | `/students`          | Récupérer tous les étudiants.           |
| POST    | `/students/save`     | Ajouter un nouvel étudiant.             |
| DELETE  | `/students/delete/{id}` | Supprimer un étudiant par son ID.     |
| GET     | `/students/count`    | Obtenir le nombre total d'étudiants.    |
| GET     | `/students/byYear`   | Nombre d'étudiants par année de naissance.|

---

## Technologies Utilisées
- **Backend** : Spring Boot (Spring Data JPA, Spring Web).
- **Base de Données** : MySQL.
- **Build Tool** : Maven.
- **Documentation API** : Swagger OpenAPI (annotations incluses).

---

## Auteur
- **Hafsa Azizi**  

---
