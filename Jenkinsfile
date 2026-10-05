pipeline {
    agent {
      label 'node1'
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh '/opt/building-a-multibranch-pipeline-project/jenkins/scripts/test.sh'
            }
        }
    }
}
