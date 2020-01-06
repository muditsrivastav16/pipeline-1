pipeline {
	agent {
		node {
			label 'master'
		}
	}
	
	stages {
		stage ('Build') {
			steps {
				git([url: 'https://github.com/muditsrivastav16/DemoSeedJob-1.git', branch: 'master'])
				echo 'Build "${BUILD_NUMBER}"'
				bat 'javac CheckPipeline.java'
				bat 'java ChcekPipeline !'
			}
		}
	}
}
