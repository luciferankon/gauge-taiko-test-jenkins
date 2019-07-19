pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'sudo su -'
                sh 'npm install @getgauge/cli'
                sh 'npm install'
                sh 'gauge run specs'
            }
        }
    }
}