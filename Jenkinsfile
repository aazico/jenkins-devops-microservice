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
	// agent any
	aganet { docker { image 'maven:3.6.3' }}
	stages {
		stage ('Build') {
			steps {
				sh 'mvn --version'
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
	} 
	
	post {
		always {
			echo "always 50 passes"
		}
		success {
			echo "sucess 50 passes"
		}
		failure {
			echo "failure 50 passes"
		}
	}
	
}

