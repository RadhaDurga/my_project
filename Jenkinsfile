pipeline {
    agent any

    stages {
        stage('scm checkout') {
            steps {
                git 'https://github.com/RadhaDurga/my_project'
            }
        }
        stage('complile-package') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy-package') {
            steps {
                
                ansiblePlaybook(
                    playbook: '/home/ec2-user/ansible/first_play.yml'
                )    
            }
        }
    }
}
