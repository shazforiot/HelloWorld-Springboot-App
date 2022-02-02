pipeline {
    agent any
    stages {
        stage ('git clone') {
            steps {
                git 'https://github.com/HRABOVENSKYI/HelloWorld-Springboot-App.git'     
            }
        }
        stage ('create dockerimage') {
            steps {
                sh 'docker build -t springboot:latest .'     
            }
        }
    }
}
