pipeline {
    agent any
    stages {
        stage ('git clone') {
            steps {
                git 'https://github.com/HRABOVENSKYI/HelloWorld-Springboot-App.git'     
            }
        }
        stage ('maven test') {
            steps {
                bat 'mvn test'
            }
        }
        stage ('maven build') {
            steps {
                bat 'mvn package'
            }
        }
        stage ('maven deploy') {
            steps {
                echo "Deploying the war file to the server"
            }
        }
    }
}
