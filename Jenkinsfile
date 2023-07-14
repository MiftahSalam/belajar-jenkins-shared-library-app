pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Hello Build"
            }
        }
        stage("Test") {
            steps {
                echo "Hello Test"
                sh("error")
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