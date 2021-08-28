pipeline {
    agent any
    //agent { docker { image 'node:13.8'} }
    environment {
        dockerHome = tool 'myDocker'
	mavenHome  = toll 'myMaven'
	PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
    }
    stages {
        stage ('Build') {
            steps {
                sh 'mvn --version'
	        sh 'docker version'
		echo "Build"
		echo "PATH - $PATH"
		echo "BUILD_NUMBER - $env.BUILD_NUMBER"
		echo "BUILD_ID - $env.BUILD_ID"
		echo "JOB_NAME - env.JOB_NAME"
		echo "BUILD_TAG - env.BUILD_TAG"
		echo "BUILD_URL - env.BUILD_URL"
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
