pipeline {
	agent any
	stages {
		stage ('Create job') {
			job('DSL_Maven_3') {
			scm {
				git ('https://github.com/muditsrivastav16/simple-java-maven-app.git', 'master')
			}
				triggers {
				scm('* * * * *')
			  }
				publishers {
			  mailer('2015pcecsmudit@poornima.org', true, true)
			}
				steps {
					maven {
						goals('clean package')
					}
				}
			}
		}


		stage ('Build') {
			steps {
				echo 'Build'
			}
		}
	}

	
}




  
  
  
