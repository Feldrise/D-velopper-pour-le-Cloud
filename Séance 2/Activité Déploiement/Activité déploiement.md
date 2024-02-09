# Activité de déploiement dans le Cloud

## Objectifs
L'objectif de cette activité est de vous familiariser avec le déploiement d'applications sur des plateformes de cloud public, en l'occurrence Google Cloud Platform (GCP) et Amazon Web Services (AWS). Vous travaillerez sur un projet comprenant un frontend en React et un backend en Python, sans base de données. Cette activité renforcera votre compréhension de la gestion de machines virtuelles et de la configuration nécessaire pour déployer une application web moderne.

## Prérequis
- Compte actif sur Google Cloud Platform et Amazon Web Services.
- Connaissances de base en utilisation de Git pour cloner un répertoire.
- Familiarité avec les commandes de base Linux pour la configuration de serveurs.
- Connaissances élémentaires de React et Python.

## Instructions

### Partie 1: Préparation
1. **Cloner le répertoire GitHub** : Commencez par cloner le répertoire suivant : [https://github.com/langchain-ai/opengpts](https://github.com/langchain-ai/opengpts). Ce répertoire contient le code source du frontend (React) et du backend (Python) de l'application à déployer.

2. **Examen du code** : Familiarisez-vous avec la structure du code et les Dockerfiles inclus. Ces derniers vous fourniront des indices sur la configuration requise pour les environnements de votre application, même si vous ne les utiliserez pas directement pour cette activité.

### Partie 2: Déploiement sur Google Cloud Platform (GCP)
1. **Création d'une instance de VM (Virtual Machine)** : Utilisez Google Cloud Console pour créer deux instances de VM, une pour le frontend et une pour le backend. Sélectionnez une configuration adaptée (par exemple, e2-medium) et une image de système d'exploitation (Ubuntu recommandé).

2. **Configuration de l'instance** : Connectez-vous à vos instances via SSH. Installez les dépendances nécessaires, telles que Node.js pour le frontend et Python pour le backend. Utilisez les Dockerfiles comme guide pour les dépendances spécifiques.

3. **Déploiement du frontend** : Sur l'instance dédiée au frontend, clonez à nouveau le répertoire, naviguez dans le dossier du frontend, installez les dépendances avec `npm install` et lancez l'application avec `npm start`.

4. **Déploiement du backend** : Répétez un processus similaire sur l'instance backend : installez Python, les dépendances nécessaires, et lancez le serveur backend.

5. **Vérification et test** : Assurez-vous que le frontend peut communiquer avec le backend. Testez l'application en accédant à l'adresse IP publique de l'instance frontend via un navigateur.

### Partie 3: Déploiement sur Amazon Web Services (AWS)
1. **Création d'instances EC2** : Identique à l'étape GCP, créez deux instances EC2 pour le frontend et le backend, en choisissant une configuration similaire et une image Amazon Linux 2 ou Ubuntu.

2. **Configuration et déploiement** : Suivez les mêmes étapes de configuration et de déploiement que pour GCP, en adaptant les commandes si nécessaire pour l'environnement AWS.

3. **Vérification et test** : Comme avec GCP, testez l'accès au frontend et assurez-vous qu'il communique correctement avec le backend.

## Livrables
- URL d'accès au frontend de votre application déployée sur GCP et AWS.
- Brève documentation décrivant les étapes que vous avez suivies, toute difficulté rencontrée et comment vous l'avez surmontée.

## Évaluation
Votre travail sera évalué sur la base de :
- La réussite du déploiement sur les deux plateformes.
- La clarté et la précision de votre documentation.
- Votre capacité à surmonter les obstacles techniques.

## Conseils
- Consultez la documentation officielle de GCP et AWS pour des détails spécifiques sur la création d'instances et la configuration des services.
- Utilisez les Dockerfiles comme référence pour les dépendances requises, même si vous ne les utilisez pas pour la conteneurisation.
- N'hésitez pas à demander de l'aide sur les forums ou dans la documentation en cas de blocage.

---

Bon courage ! 🚀 Vous êtes sur le point de franchir une étape importante dans le développement de vos compétences en déploiement cloud.