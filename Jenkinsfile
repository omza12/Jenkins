pipeline {
	//agent any
	//agent {docker { image 'maven:3.6.3'}}
	agent {docker { image 'node:13.8'}}
	stages{		
		stage('Build') {
			steps{
				//sh 'mvn --version'
				sh 'node --version'
				echo "Build"
			}
		}
		stage('Test') {
			steps{
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps{
				echo "Integration Test"
			}
		}
	} 
	post {
		always {
			echo "always run"
		}
		success{ 
			echo "run when succes"
		}
		failure {
			echo "run when fail"
		}
	}
}
