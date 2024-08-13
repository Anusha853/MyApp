pipeline {
    agent any
    environment {
        PATH = "C:/Users/e040106/Downloads/apache-maven-3.9.8-bin/apache-maven-3.9.8/bin;${env.PATH}"
    }
    stages {
        stage('Checkout') {
            steps {
                git "https://github.com/Anusha853/MyApp.git"
            }
        }
        stage('Test'){
            steps {
                bat "mvn test"
            }
        }
        stage('Install'){
            steps{
                bat "mvn install"
            }
        }
    }
}
