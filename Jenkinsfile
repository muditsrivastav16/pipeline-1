pipeline {
	agent any
	stages {
		stage ('createing job') {
		steps {
			job('DSL_Maven3') {
				scm {
    git {
      remote {
        url 'https://github.com/muditsrivastav16/simple-java-maven-app.git'
      }
      branch 'master'
    }
  }
  triggers {
    scm('* * * * *')
  }
  
  publishers {
        mailer('2015pcecsmudit@poornima.org', true, true)
    }
			}
  steps {
    maven {
      goals('clean package')
	  batchFile('mvn -Dmaven.test.failure.ignore=true install')
      batchFile('echo Hello')
    }}
  }
}
	}
