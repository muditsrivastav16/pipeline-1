pipeline
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
        
