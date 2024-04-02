pipeline {
    agent any
    
    stages {
        stage('Git Checkout') {
            steps {
                echo 'Checking out code from Git'
                git branch: '*/master', url: 'https://github.com/simplilearn-github/Pipeline_Script.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project'
                // Add your build commands
            }
        }
        // Add more stages as needed
    }
    
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
    }
}
