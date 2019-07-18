/*
pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        }
    }
}
------------------------------------------------------
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Build result') {
            steps {
                echo 'Build Successfull'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
---------------------------------------------------------------------
node {
    checkout scm
}

--------------------------------------------------------------------
pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                bat 'make'
                archiveArtifacts artifacts: '**./target/.*.jar', fingerprint: true [there is no . between *./ and /.*]
            }
        }
    }
}
--------------------------------------------------------------------




pipeline {
agent any
       stages {
           stage ('String') {
               def name = 'mudit'
               steps {
                  
                   echo 'Hello ${name}'
                    echo "hello ${name}"
                }
            }
        }
    }            
    
    ----------------------------------------------------------
    
    */

pipline {
    agent any
    stages {
        stage ('Example') {
            steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
    }
}
