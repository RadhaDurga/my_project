node{
    stage('SCM checkout'){
    git' https://github.com/RadhaDurga/my_project'
    }
    stage('complile-package'){
    sh 'mvn clean package'
    }
    stage('Deploy-package'){
    sh ansible-playbook deploy_file.yml
    }      
    }
