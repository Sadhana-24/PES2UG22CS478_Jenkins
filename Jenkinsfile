pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the C++ application...'
                sh 'g++ -o PES2UG22CS478-1 main/hello.cpp'
                echo 'Build completed successfully!'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing the C++ application...'
                sh './PES2UG22CS478-1'
                echo 'Testing completed successfully!'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the C++ application...'
                echo 'Deployment completed successfully!'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed!'
        }
        success {
            echo 'Pipeline executed successfully!'
        }
    }
}