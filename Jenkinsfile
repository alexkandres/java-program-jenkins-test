pipeline {
    agent any
    
    environment {
        AWS_ACCESS_KEY_ID = credentials('testAccessKey')   
    }
    
    stages {
        stage('Test') {
            steps {
                    bat 'set'
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
