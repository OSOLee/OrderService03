pipeline {
    agent any

    tools {
        maven 'my-maven'
    }

    stages {
        stage('0. 자동화2 연결확인') {
            steps {
                echo '스테이지 출발'
            }
        }

        stage('1. Maven Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        
        stage('2. Check Docker1') {
            steps {
                sh 'docker version'
            }
        }
        
        stage('3. Docker build') {
            steps {
                sh 'docker buildx build -t order-service03-app:latest .'
            }
        }
    }
}