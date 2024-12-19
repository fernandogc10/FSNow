pipeline {
    agent any

     triggers {
        githubPush() 
    }

    stages {
        stage('Print message') {
            steps {
                echo "Clonando repositorio..." 
            }
        }

        stage('Checkout'){

            git branch: 'main', url: 'https://github.com/usuario/repositorio-publico.git'

        }

        stage('ls'){
            echo "Viendo archivos..."
            sh 'ls -la'
        }
        
    }
}