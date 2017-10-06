pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                retry(3){
                    bat 'echo hiiiiiiiiiiiiiiiiiiiii'
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
    }
}
