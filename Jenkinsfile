pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                git url: 'https://github.com/surajkumarsingh03/Bitcoin-Prices-Prediction-Using-DNN-Techniques'
            }
        }

        stage('Build') {
            steps {
                // Install dependencies (adjust based on your project's needs)
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                // Run your project tests or any other verification
                sh 'python -m unittest discover tests'
            }
        }

        stage('Deploy') {
            steps {
                // Steps for deployment (optional)
                echo 'Deploying application...'
            }
        }
    }
}
