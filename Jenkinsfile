pipeline {
    agent {
        label "java-slave"
    }
    stages {
        stage ('This executed in JAVA-Machine') { 
            steps {
                script {
                    sh 'java -version'
                }
            }
        }
        stage ('This Executed in Docker-Machine') {
            agent {
                label 'docker-slave'
            }
            steps {
                script {
                    sh 'docker version'
                }
            }
        }
    }
}
