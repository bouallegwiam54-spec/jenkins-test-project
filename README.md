# jenkins-test-project
pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Code récupéré depuis GitHub!'
            }
        }
        stage('Build') {
            steps {
                echo 'Construction du projet...'
                sh 'echo "Build en cours..."'
            }
        }
        stage('Test') {
            steps {
                echo 'Tests en cours...'
                sh 'echo "Tous les tests sont OK!"'
            }
        }
    }
}
