pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                echo "Building"
            }
        }
        stage ('Test') {
            steps {
                echo "Testing"
            }
        }
        stage ('Deploy') {
            steps {
                echo "Deploying"
            }
        }
    }
    post {
        always {
            echo 'I'm awesome. I run always'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    }
}
