pipeline {
    agent { docker 'php' }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
                sh 'php yii serve --port=8888'
            }
        }
    }
}
