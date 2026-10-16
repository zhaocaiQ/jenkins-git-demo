pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Git 저장소에서 코드를 가져왔습니다.'
            }
        }
    }

    stage('Test') {
        steps {
            bat 'python --version'
            bat 'python main.py'
        }
    }

    stage('Build') {
        steps {
            echo '빌드 단계 성공'
        }
    }

    post {
        success {
            echo 'CI 파이프라인 성공!'
        }

        failure {
            echo 'CI 파이프라인 실패. 로그를 확인하세요.'
        }
    }
}