pipeline {
    agent any 

    stages {

        stage('Checkout') {
            steps {
                echo "Checkout from git is successfull"
            }
        }

        stage('Install dependencies') {
            steps {
                echo 'Install dependencies successfull'
            }
        }
        
        stage('Echo message') {
            steps {
                echo "-------------------------------------------- MASTER ------------------------------------------------------------"
            }
        }

        stage('Run unitTest') {
            steps {
                sh 'python3 -m unittest discover'
            }
        }

        stage('deploy code') {
            steps {
                echo "deploy to ECR"
            }
        }
    }

}