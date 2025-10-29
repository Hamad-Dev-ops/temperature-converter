pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                echo 'Building Temperature Converter Project...'
                sh 'npm run build'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running Tests...'
                sh 'npm test'
            }
        }
        
        stage('Package') {
            steps {
                echo 'Packaging the application...'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}
