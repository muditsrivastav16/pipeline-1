pipeline {
	agent {
		node {
			label 'master'
		}
	}
	
	stages {
		stage ('Build') {
			steps {
				git([url: 'https://github.com/muditsrivastav16/DemoSeedJob-1.git', branch: "${params.BRANCH}"])
				echo 'Build "${BUILD_NUMBER}"'
				bat 'javac CheckPipeline.java'
				bat "java CheckPipeline ${params.BRANCH}"
			}
		}
	}
}
