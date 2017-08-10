pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'composer install'
                sh 'echo "Build Success"'
            }
        }
        stage('Test') {
            steps {
                sh 'php yii serve --port=8888'
                sh 'echo "Test Success"'
            }
        }
    }
}
