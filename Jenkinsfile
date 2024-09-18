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
                ok "deployer"
                submitter "admin devops"
                submitterParameter "USER_SUBMIT"
                parameters {
                    string(name: "VERSION", defaultValue: "latest", description: "input test")
                }
            }
            steps {
                echo "user: ${ USER_SUBMIT }"
                echo "version : ${ VERSION }"
                echo "deploy"
            }
        }
    }
}