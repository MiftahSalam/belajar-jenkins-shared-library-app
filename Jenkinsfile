pipeline {
    agent any
    }
    stages {
        stage("Build") {
            steps {
                echo "Hello Build"
            }
        }
        stage("Tes") {
            steps {
                echo "Hello Test"
            }
        }
        stage("Deploy") {
            steps {
                echo "Hello Deploy"
            }
        }
    }
    post {
        always {
            echo "always executed"
        }
        success {
            echo "execute success step"
        }
        failure {
            echo "execute failure step"
        }
        cleanup {
            echo "cleaning up"
        }
    }
}