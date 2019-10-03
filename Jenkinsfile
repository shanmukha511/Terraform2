pipeline{
    agent any
    stages
    {
    stage('test')
    {
        steps{
            //git branch: 'master',
              //  credentialsId: 'Token',
                //url: 'https://github.com/shanmukha511/Terraform.git'
 checkout scm
            
      
            
     sh "cp /var/tmp/vars.tf /var/jenkins_home/workspace/new_test/"
            sh 'terraform init -input=false '
                            sh 'terraform plan '
        }
    }
}
}
