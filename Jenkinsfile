pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Hello") {
            steps {
                echo "Hello Pipeline"
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