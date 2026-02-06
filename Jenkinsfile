pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git branch: 'main', url: 'https://github.com/Sriram-190/aws-capstone-exam.git'
      }
    }
    stage('Deploy via Ansible') {
      steps {
        sh 'ansible-playbook -i ansible/hosts.ini ansible/playbook.yml'
      }
    }
  }
}
