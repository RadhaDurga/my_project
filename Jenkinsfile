pipeline {
    agent any

    stages {
        stage('scm checkout') {
            steps {
                git 'https://github.com/RadhaDurga/Automation-Project.git'
            }
        }
        stage('complile-package') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Deploy-package') {
            steps {
                echo "Deploy Successfull"
                 
            }
        }
    }
}
