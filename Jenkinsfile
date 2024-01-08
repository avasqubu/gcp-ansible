pipeline {
  agent any

  stages {
    stage('Ansible') {
      steps {
        script {
            ansiblePlaybook(            
                playbook: 'playbook.yaml',
                inventory: 'inventory',
                credentialsID: 'JenkinsSSH',
                disableHostKeyChecking: true,
                vaultTmpPath:''
                )       
              }
            }
        }
    }
}
