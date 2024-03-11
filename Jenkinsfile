pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file using a shell script
                sh 'ls'
                build 'PES2UG21CS479-1'
                sh 'g++ -o obj main/hello.cpp'
            }
        }

        stage('Test') {
            steps {
                // Print the output of the compiled .cpp file
                sh './ob'
            }
        }

        stage('Deploy') {
            steps {
              echo 'deploy'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
