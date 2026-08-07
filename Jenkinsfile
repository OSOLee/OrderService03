pipeline {
    agent any

	tools{
		maven 'my-maven'
	}
    stages {
        stage('0. 연결확인') {
            steps {
                echo '스테이지 출발'
            }
        }
        
        stage('1. 자바빌드'){
			steps{
				echo '메이븐으로 빌드를 시작'
			}
		}
    }
}