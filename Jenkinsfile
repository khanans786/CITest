pipeline {
    agent any
     
    stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/khanans786/CITest.git'
             
          }
        }

        
        
        
        stage('Ansible Execute') {
             
            steps {
                 
                ansiblePlaybook credentialsId: 'Ansible-Key', disableHostKeyChecking: true, installation: 'ansible2', inventory: 'dev.inv', playbook: 'apache.yml'

}
}
}
}
