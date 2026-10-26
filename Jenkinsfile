
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Jenkins Pipeline 시작'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo '소스 코드 확인 완료'
            }
        }

        stage('Test') {
            steps {
                echo '테스트 단계 실행 완료'
            }
        }
    }
}
