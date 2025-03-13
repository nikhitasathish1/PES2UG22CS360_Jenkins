pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o main/PES2UG22CS360 main/hi.cpp' // Compile hello.cpp
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './main/PES2UG22CS360' // Run the compiled executable
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...' // Simulate deployment
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
