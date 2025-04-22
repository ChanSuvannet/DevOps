pipeline {
    agent { label 'laravel-agent' } // must match your Docker label
    stages {
        stage('Prepare Env') {
            steps {
                sh 'cp .env.example .env'
            }
        }
        stage('Composer Install') {
            steps {
                sh 'composer install'
            }
        }
    }
}
