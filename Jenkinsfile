
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
    
    stage("vars copy"
          {
              steps
              {
                  sh "cp /var/tmp/vars.tf /var/jenkins_home/workspace/new_test/"
              }
          }
        stage('terraform init') {
            steps {
                sh 'terraform init -input=false '
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
