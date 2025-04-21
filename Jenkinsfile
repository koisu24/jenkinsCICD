pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }

        stage('Build') {
            steps {
                echo '✅ Build 단계 - 생략 가능'
            }
        }

        stage('Deploy') {
            steps {
                echo '🚀 배포 단계 - 지금은 모의로 처리 중'
            }
        }
    }

    post {
        success {
            echo '🎉 파이프라인이 성공적으로 완료되었습니다!'
        }
        failure {
            echo '❌ 실패! 로그를 확인해보세요.'
        }
    }
}
