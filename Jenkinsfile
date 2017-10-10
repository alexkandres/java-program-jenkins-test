pipeline {
    agent any
    
    stages {
        stage('Test') {
            steps {
                    bat 'set'
            }
        }
    }
    
    post {
        always {
            junit "build/reports/**/*.xml"
        }
        
    }
}
