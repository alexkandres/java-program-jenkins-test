pipeline {
    agent any
    
    environment {
        AWS_ACCESS_KEY_ID = credentials('AWS_ACCESS_KEY_ID')   
    }
    
    stages {
        stage('Test') {
            steps {
                    bat 'set'
                    bat 'dir'
                    dir('folder4') {
                        // some block
                        bat 'dir'
                    }

                    
            }
        }
    }
    
    post {
        always {
            echo "always: if this shows always is workinf"
        }
        success {
            echo "Success: only run if build was success"   
        }
        failure {
            echo "failure: only when build fails"   
        }
        changed {
            echo "changed: only when build chenges"   
        }
    }
}
