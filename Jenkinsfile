pipeline {
    agent any


    stages {
        stage('build') {
            steps {
                echo "build"
            }
        }

        stage('deployment production') {
            input {
                message "Voulez-vous déployer en production ?"
            }
            steps {
                echo "deploy"
            }
        }
    }
}