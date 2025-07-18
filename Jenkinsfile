pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'deploy-docker', url: 'https://github.com/GAUTAM7978/Task4-2.0.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i inventory playbook.yml'
            }
        }
    }
}
