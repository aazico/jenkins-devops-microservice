// SCRIPTED
// node {
	// SCRIPTED I
	// stage('Build') {
	// 	echo "Build"
	// }
	// stage('Test') {
	// 	echo "Test"
	// }
	// stage('Integration Test') {
	// 	echo "Integration Test"
	// }

	// SCRIPTED II
	// echo "Build"
	// echo "Test"
	// echo "Integration Test"
// } 

// DECLARATIVE
pipeline {
	agent any
	stages {
		stage ('Build') {
			steps {
				echo "Build"
			}
		}
		stage ('Test') {
			steps {
				echo "Test"
			}
		}
		stage ('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} post {
		always {
			echo 'always 50 passes'
		}
		sucess {
			echo 'sucess 50 passes'
		}
		failure {
			echo 'sucess 50 passes'
		}
	}
	
}

