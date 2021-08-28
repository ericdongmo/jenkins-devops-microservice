pipeline {
    //agent any
    agent { docker { image 'maven:3.6.3'} }
    stages {
        stage ('Build') {
            steps {
                sh 'mvn --version'
            }
        }
        stage ('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
        stage ('Dev') {
            steps {
                echo 'Development'
            }
        }
        stage ('Ship') {
            steps {
                echo 'Shipment'
            }
        }
    }
}
