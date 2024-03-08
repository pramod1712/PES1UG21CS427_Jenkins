pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ hello2.cpp -o temp'
                 build job: 'PES1UG21CS427-1', wait: false
                 echo 'Build by CS427 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat hello2.cpp'
                echo 'Test by CS427 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 echo 'Deploy by CS427 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
