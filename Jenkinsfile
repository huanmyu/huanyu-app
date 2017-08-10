pipeline {
    agent { docker 'php' }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
                sh 'docker run --rm --interactive --tty --volume $PWD:/app --user $(id -u):$(id -g) composer install'
            }
        }
    }
}
