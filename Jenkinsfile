
pipeline{
  agent any
  
  stages {

    stage('Cloning Git') {
       steps {
         ansiblePlaybook disableHostKeyChecking: true, installation: 'ansible', inventory: '/var/deployment/hosts', playbook: '/var/deployment/main.yml', vaultCredentialsId: 'ansible vault password'
        }
     }
     
   }
    
}
