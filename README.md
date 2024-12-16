# Projet Spring Boot : Gestion des Étudiants

## Description
Ce projet est une application RESTful développée avec Spring Boot pour gérer les étudiants. Il propose des fonctionnalités telles que la création, la suppression, la récupération et le comptage des étudiants. Les données sont persistées dans une base de données MySQL.

---

## Fonctionnalités
- **Ajout d'un étudiant** : Enregistrement des informations d'un étudiant (nom, prénom, date de naissance).
- **Suppression d'un étudiant** : Suppression d'un étudiant par son ID.
- **Récupération des étudiants** : Liste de tous les étudiants.
- **Comptage des étudiants** : Nombre total d'étudiants enregistrés.
- **Statistiques** : Nombre d'étudiants par année de naissance.

---

## Prérequis
- Java 17 ou supérieur.
- MySQL installé et configuré.
- Maven 3.8 ou supérieur.
- Outil de développement (IntelliJ, Eclipse, etc.).

---

## Installation
1. Clonez ce dépôt :
   ```bash
   git clone https://github.com/HafsaAzizi/spring-boot.git .
   ```
2. Configurez la base de données MySQL :
   - Créez une base de données nommée `studentdb`.
   - Mettez à jour le fichier `application.properties` si nécessaire :
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/studentdb?serverTimezone=UTC
     spring.datasource.username=VotreNomUtilisateur
     spring.datasource.password=VotreMotDePasse
     ```
3. Installez les dépendances et lancez l'application :
   ```bash
   mvn spring-boot:run
   ```

---

## Utilisation
Pour démarrer l'application :
1. Clonez le projet, puis lancez l'application avec la commande :
   ```bash
   mvn spring-boot:run
   ```
2. Accédez à l'interface **Swagger UI** pour interagir avec l'API :
   [Swagger UI](http://localhost:8080/swagger-ui/) :  
   L'interface vous permet de tester les différents points de terminaison de l'API et de visualiser la documentation.

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
- **Documentation API** : Swagger OpenAPI.

---



https://github.com/user-attachments/assets/dc1f8cd2-cac5-401b-9739-8e208c51caf8



https://github.com/user-attachments/assets/d2857acf-5d85-4de1-9402-beae6b722a71





## Auteur
- **Hafsa Azizi**  

---
