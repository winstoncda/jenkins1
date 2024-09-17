pipeline {
    agent any

    environment {
        MY_USERNAME = "olidev"
        MY_PASSWORD = "*****"
    }

    stages {
        stage('build') {
            steps {
                echo "BRANCH_NAME : ${ env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY : ${ env.BRANCH_IS_PRIMARY}"
                echo "CI : ${ env.CI }"
                echo "BUILD_NUMBER : ${ env.BUILD_NUMBER}"
                echo "JENKINS_URL : ${ env.JENKINS_URL}"
                echo "MY_USERNAME : ${ env.MY_USERNAME}"
                echo "MY_PASSWORD : ${ env.MY_PASSWORD}"
                sh 'printenv'
            }
        }
    }
}