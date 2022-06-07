pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git 'https://github.com/siddvi/ansible-playbook'
            }
        }
        stage('Hi') {
            steps {
                ansiblePlaybook credentialsId: 'c31a425f-201e-4b56-bc2d-2b9a86c3ec6a', disableHostKeyChecking: true, installation: 'Ansible', playbook: 'test-playbook3.yaml'
            }
        }
    }
}
