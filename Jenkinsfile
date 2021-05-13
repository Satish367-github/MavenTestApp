pipeline {
    agent any

    stages {
        stage('Clean') {
            steps {
                echo 'Cloning and Cleaning Repo'
                sh "mvn clean"
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing the App...'
                sh "mvn test"
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the App...'
                sh "mvn package"
            }
        }
    }
}
