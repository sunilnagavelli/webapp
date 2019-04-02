pipeline {
    agent any
    stages {
        stage('Initialize') {
            steps {
                checkout scm
                script {
                   echo "Hello"
                    sh 'ls -l'
                    sh '''
                        mvn clean package
                        ls -l
                    '''
                }
            }
        }
    }
}
