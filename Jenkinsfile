pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/shazforiot/HelloWorld-Springboot-App.git'
            }
        }
        stage('Create Dockerimage'){
            steps{
                sh 'dpcker build -t thetips4you/springboot:latest .'
            }
        }
        
    }
}
