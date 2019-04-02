pipeline {
    agent any
    stages {
        stage('Initialize') {
            steps {
                checkout scm
                script {
                    sh '''
                        ls
                        ${M2_HOME}/bin/mvn clean package
                        ls -l
                    '''
                }
            }
        }
    }
}
