pipeline {
    agent any
    tools {
        maven 'Maven3'
        jdk 'jdk8'
    }
    stages {
        stage('Initialize') {
            steps {
                checkout scm
                script {
                    sh '''
                        ls
                        echo "PATH = ${PATH}"
                        echo "M2_HOME = ${M2_HOME}"
                        mvn clean package
                        ls -l
                    '''
                }
            }
        }
    }
}
