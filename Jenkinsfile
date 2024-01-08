pipeline {
  agent any

  stages {
    stage('Ansible') {
      steps {
        script {
            ansiblePlaybook
                playbook: 'playbook.yml'
                inventory: 'inventory'
                credentialsID: 'JenkinsSSH'
                disableHostKeyChecking: true
                vaultTmpPath:''
                }
            }
        }
    }
}
