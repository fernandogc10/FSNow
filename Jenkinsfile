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
                checkout scm
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
