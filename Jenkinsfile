pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                
                git 'https://github.com/mostafa-7ussein/nodetask'
            }
        }
        stage('Install Ansible') {
            steps {
                
                sh 'sudo apt-get update && sudo apt-get install -y ansible'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                
                sh 'ansible-playbook ansible-playbook.yml'
            }
        }
    }
}
