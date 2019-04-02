pipeline {
    agent any
    stages {
        stage('Initialize') {
            steps {
                checkout scm
                script {
                   echo "Hello"
                    sh 'ls -l'
                }
            }
        }
    }
}
