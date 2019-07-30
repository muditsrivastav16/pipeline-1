pipeline {
	agent any
	options {
			timestamps() 
		}
	
	triggers {
		cron('* * * * *')
	}
	
	stages {		
		stage ('createing job') {
			steps {
				echo 'creating job'
			}
		}
		stage ('setting maven') {
  		steps {
				echo 'setting maven'
  		}
		}
	}
}
