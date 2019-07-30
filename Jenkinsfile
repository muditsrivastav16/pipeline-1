pipeline {
	agent any
	options {
			timestamps() 
		}
	
	triggers {
		corn('* * * * *')
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
