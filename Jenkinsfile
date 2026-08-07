pipeline {
    agent any

    tools {
        maven 'my-maven'
    }

    stages {
        stage('0. 연결확인') {
            steps {
                echo '스테이지 출발'
            }
        }

        stage('1. Maven Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}