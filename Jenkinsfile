pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'su - npm install @getgauge/cli'
                sh 'su - npm install'
                sh 'su - gauge run specs'
            }
        }
    }
}