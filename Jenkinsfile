pipeline {
	agent any	
	stages {
		stage ('CreateJob') {
			steps {
				job('Maven_3') {
					scm {
						git ('https://github.com/muditsrivastav16/simple-java-maven-app.git', master)
						
						
					}
				}
				echo 'job created'
			}
		}
	}
}
