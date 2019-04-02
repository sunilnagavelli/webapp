pipeline {
    agent any
    tools {
        maven 'Maven3
    }
    stages {
        stage('Initialize') {
            steps {
                checkout scm
                script {
                    sh '''
                        ls
                        echo ${M2_HOME}
                        ${M2_HOME}/bin/mvn clean package
                        ls -l
                    '''
                }
            }
        }
    }
}
