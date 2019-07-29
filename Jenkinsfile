pipeline {
    
    job('DSL_Maven_pipeline') {
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
                    echo 'Build'
                }
    
    agent any
    stages {
        stage ('Build') {
            steps {
                echo 'Build'                
            }
        }
        stage ('Test') {
            steps {
                echo 'Test'
                maven {
                    goals ('clean package')
                }
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
}
        
