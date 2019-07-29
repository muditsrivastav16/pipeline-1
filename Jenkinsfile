pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                job ('MavenJobPipeline') {
                    scm {
                        giturl('https://github.com/muditsrivastav16/simple-java-maven-app.git')
                        branch 'master'
                    }
                }
                echo 'Build'                
            }
        }
        stage ('Test') {
            steps {
                echo 'Test'
            }
        }
        stage ('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
}       
