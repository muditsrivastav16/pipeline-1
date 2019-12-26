pipeline {
	agent {
		node {
			label 'master'
		}
	}
	
	stages {
		stage ('Build') {
			steps {
				git([url: 'https://github.com/muditsrivastav16/Shared_Library.git', branch: 'master'])
				echo 'Build "${BUILD_NUMBER}"'
			}
		}
	}
}
