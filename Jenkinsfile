pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..2'
                sh 'javac HelloWorld.java'
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'java HelloWorld'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'ls -ltr'
                sh 'rm /var/lib/jenkins/workspace/pipeline_5th_jenkinsfile/*'
            }
        }
    }
}
