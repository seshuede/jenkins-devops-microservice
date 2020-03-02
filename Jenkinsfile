// Scripted Pipeline

// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('Integration Test') {
// 		echo "Integration Test"
// 	}
// }


// Declarative

pipeline {
	agent any
	stages {

		stage('Build') {
			steps {
				echo "Build"
			}
		}

		stage('Test') {
			steps {
				echo "Test"
			}
		}

		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}

	post {
		always {
			echo 'Im awsome, I run always'
		}
		success {
			echo 'I run when u r succesful'
		}
		failure {
			echo 'I run when u fails'
		}
		//changed success -> fail / fail -> success
	}
}
