pipeline {
	agent any	
	stages {
		stage ('CreateJob') {
			steps {
				job('Maven_3') {
					scm {
						git {
							url 'https://github.com/muditsrivastav16/simple-java-maven-app.git'
							branch 'master'
						}
					}
				}
				echo 'job created'
			}
		}
	}
}
