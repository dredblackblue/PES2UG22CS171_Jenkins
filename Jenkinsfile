pipeline {
    agent any  // Runs on any available agent

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building C++ Project...'
                    sh 'g++ -o output main.cpp' // Compiling C++ file
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo 'Running Tests...'
<<<<<<< HEAD
                    sh './output'  // Execute compiled binary
=======
                    sh './non_existent_binary'  // Intentional error: File does not exist
>>>>>>> 6ba87d4 (Introduced error in Test stage to verify failure handling)
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying...'
                    echo 'Deployment Successful ✅'
                }
            }
        }
    }

    post {
        failure {
            echo '🚨 Pipeline Failed! Check logs for errors.'
        }
    }
}
<<<<<<< HEAD
=======

>>>>>>> 6ba87d4 (Introduced error in Test stage to verify failure handling)
