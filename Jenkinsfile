pipeline {
  agent any
  stages {
    stage('pull SCM') {
      steps {
        git(url: 'https://github.com/sjpillai/Jenkinsrepo1.git', branch: 'main', credentialsId: 'sjpillai')
      }
    }

    stage('Terraform init') {
      steps {
        bat 'terraform init'
      }
    }

    stage('Deploy') {
      steps {
        bat 'echo "blue ocean script executed"'
      }
    }

  }
}