pipeline {
    agent {
        docker {image 'node:7-alpine'}   
    }
    stages {
        stage('Test') {
            steps {
                    bat 'echo hiiiiiiiiiiiiiiiiiiiii'
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
