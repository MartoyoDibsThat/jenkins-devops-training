pipeline {
    //agent any
    agent {
        docker {
            image 'maven:3.6.3'  
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
    post {
        always {
            echo 'runs always'
        }
        success {
            echo 'runs on success'
        }
        failure {
            echo 'runs on failure'
        }
    }
}