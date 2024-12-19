pipeline {
    agent any
    //test

    triggers {
        githubPush()
    }

    stages {
        stage('Print message') {
            steps {
                echo "Clonando repositorio..."
            }
        }

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/fernandogc10/FSNow.git'
            }
        }

        stage('ls') {
            steps {
                echo "Viendo archivos..."
                sh 'ls -la'
            }
        }
    }
}
