pipeline {
    agent any

    environment {
        MY_USERNAME = "olidev"
        MY_PASSWORD = "*****"
    }

    options { 
        timeout(time: 1, unit: 'HOURS')
        timestamps() 
    }

    parameters {
        string(name: "NAME", defaultValue: "M. Jenkins", description: "Product Owner")
        text(name: "TEXT", defaultValue: "Réunion de concertation", description: "texte de description")
        booleanParam(name: "DONE", defaultValue: true, description: "true or false")
        choice(name: "CHOICE", choices: ['design', 'development', 'deployment'], description: "Liste des tâches")
        password(name: "PASSWORD", description: "Mot de passe de connexion")
    }

    stages {
        stage('build') {
            steps {
                echo "NAME : ${ NAME}"
                echo "TEXT : ${ TEXT}"
                echo "DONE : ${ DONE}"
                echo "CHOICE : ${ CHOICE}"
                echo "PASSWORD : ${ PASSWORD}"
            }
        }
    }
}