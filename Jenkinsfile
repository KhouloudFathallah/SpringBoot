pipeline {
    agent any
    triggers {
        pollSCM('*/5 * * * *') // Vérifier toutes les 5 minutes
    }
    stages {
        stage('Checkout') {
            steps {
                echo "Récupération du code source"
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo "Build du projet"

               // sh './mvnw clean package'
            }
        }
        stage('Deploy') {
            steps {
                echo "Déploiement du projet"

                // Commandes de déploiement pour un projet Spring Boot
               // sh 'java -jar target/gestionCatalogue5Gr1.jar'
            }
        }
    }
}
