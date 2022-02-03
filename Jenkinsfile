pipeline {
    agent any
    stages {
        stage ('git clone') {
            steps {
                git 'https://github.com/HRABOVENSKYI/HelloWorld-Springboot-App.git'     
            }
        }
        stage ('maven build') {
            steps {
                bat 'mvn package'     
            }
        }
        stage ('create dockerimage') {
            steps {
                bat 'docker build -t springboot:latest .'     
            }
        }
    }
}
