pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'main', credentialsId: 'sjpillai', url: 'https://github.com/sjpillai/Jenkinsrepo1.git'
            }
        }
        stage('terra') {
            steps {
                bat 'terraform init'
            }
        }
    }
}
