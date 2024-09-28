pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/mostafa-7ussein/nodetask'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook ansible-playbook.yml'
            }
        }
    }
}
