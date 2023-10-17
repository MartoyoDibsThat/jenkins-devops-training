pipeline {
    //agent any
    agent {
        docker {
            image 'maven:latest'  
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