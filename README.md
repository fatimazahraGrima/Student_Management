# Student Management

Une application Spring Boot pour gérer les informations des étudiants, incluant des fonctionnalités d'ajout, de suppression, de récupération, et de comptage des étudiants.

---

## Table des matières
1. [Technologies utilisées](#technologies-utilisées)  
2. [Prérequis](#prérequis)  
3. [Installation](#installation)  
4. [Fonctionnalités](#fonctionnalités)  
5. [Structure du projet](#structure-du-projet)  

---

## Technologies utilisées
- **Java** : JDK 11+  
- **Spring Boot** : Framework pour créer des applications Java rapides et sécurisées.  
- **Hibernate/JPA** : Gestion des entités et de la persistance.  
- **H2 Database** : Base de données embarquée pour faciliter le développement et les tests.  
- **Maven** : Gestion des dépendances et du cycle de vie du projet.  

---

## Prérequis
1. Java JDK 11 ou une version ultérieure.  
2. Maven installé et configuré.  
3. Un IDE tel qu'IntelliJ IDEA ou Eclipse pour éditer et exécuter le projet.

---

## Installation
1. Clonez le dépôt du projet :
   ```bash
   git clone https://github.com/votre-repo/student-management.git
   cd student-management
   ```

2. Compilez et téléchargez les dépendances avec Maven :
   ```bash
   mvn clean install
   ```

3. Lancez l'application Spring Boot :
   ```bash
   mvn spring-boot:run
   ```

4. Modifiez les configurations de la base de données si nécessaire dans `src/main/resources/application.properties` :
   ```properties
spring.datasource.url=jdbc:mysql://localhost:3306/studentdb?serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=
spring.jpa.show-sql = true
spring.jpa.properties.hibernate.format_sql = true
spring.jpa.hibernate.ddl-auto = update
   ```

---

## Fonctionnalités
- Ajouter un étudiant avec ses informations personnelles.  
- Supprimer un étudiant à partir de son identifiant unique.  
- Récupérer la liste complète des étudiants.  
- Compter le nombre total d'étudiants enregistrés.  
- Rechercher des étudiants selon des critères spécifiques.  

---

## Structure du projet
```plaintext
src
├── main
│   ├── java
│   │   └── com.example.student_management
│   │       ├── controllers        # Gestion des requêtes REST
│   │       ├── entities           # Modèles de données (entités JPA)
│   │       ├── repositories       # Interfaces pour accéder à la base de données
│   │       ├── services           # Logique métier
│   │       └── StudentManagementApplication.java  # Classe principale
│   └── resources
│       ├── application.properties # Configuration du projet
│       └── static                 # Fichiers statiques (CSS, JS)
│
├── test                           # Tests unitaires et d’intégration
```

---

## Auteur
Développé par **[Fatima zahra Grimaa]**

## Video démonstrative


https://github.com/user-attachments/assets/e1423e7f-f3bf-4453-8c26-66e21253bede


