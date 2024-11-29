pipeline {
    agent {
        label 'docker-slave'
    }
    stages {
        stage ('This is interpolation stage' ) {
            steps {
                script {
                    def course = "K8S"
                    if (course == "K8S")
                    println ("welcome to ${course}")
                    else
                    println ("Please enroll to ${course}") 
                }
            }
        }
    }
}
