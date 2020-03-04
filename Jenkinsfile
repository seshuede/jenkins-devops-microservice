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

// pipeline {
// 	agent any
// 	stages {

// 		stage('Build') {
// 			steps {
// 				echo "Build"
// 			}
// 		}

// 		stage('Test') {
// 			steps {
// 				echo "Test"
// 			}
// 		}

// 		stage('Integration Test') {
// 			steps {
// 				echo "Integration Test"
// 			}
// 		}
// 	}

// 	post {
// 		always {
// 			echo 'Im awsome, I run always'
// 		}
// 		success {
// 			echo 'I run when u r succesful'
// 		}
// 		failure {
// 			echo 'I run when u fails'
// 		}
// 		//changed success -> fail / fail -> success
// 	}
// }


// Docker Image as an agent

pipeline {
	//agent { docker { image 'maven:3.6.3' } }
	agent any
	stages {

		stage('Build') {
			steps {
//				sh 'mvn --version'
				echo "Build"
				echo "BUILD_NUMBER  - $env.BUILD_NUMBER"
				echo "BUILD_ID  - $env.BUILD_ID"
				echo "JOB_NAME  - $env.JOB_NAME"
				echo "BUILD_TAG  - $env.BUILD_TAG"
				echo "BUILD_URL  - $env.BUILD_URL"
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
