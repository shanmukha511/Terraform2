
pipeline{
    agent any

stages {

        stage('terraform started') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('git clone') {
            steps {
                checkout scm
            }
        }
        stage('terraform init') {
            steps {
                sh 'terraform init '
            }
        }
        stage('terraform plan') {
            steps {
                sh 'terraform plan '
            }
        }
        stage('terraform ended') {
            steps {
                sh 'echo "Ended....!!"'
            }
        }

        
    }
}
