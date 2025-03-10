pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Building the C++ program..."
                    sh 'g++ -o PES1UG22AM167-1 hello.cpp'  // Compile C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo "Testing the compiled program..."
                    sh './PES1UG22AM167-1'  // Execute compiled program
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo "Deploying the application (Placeholder step)..."
                }
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
