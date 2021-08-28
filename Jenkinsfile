pipeline {
    //agent any
    agent { docker { image 'node:13.8'} }
    stages {
        stage ('Build') {
            steps {
               // sh 'mvn --version'
	       sh 'node --version'
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
