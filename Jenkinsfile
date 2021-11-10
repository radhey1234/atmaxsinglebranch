            
pipeline {
    agent any
    
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "GRADLE_HOME = ${GRADLE_HOME}"
                    whoami
                    gradle
                '''
            }
        }

        stage ('Build') {
            steps {
                sh 'gradle' 
            }
        }
    }
}

