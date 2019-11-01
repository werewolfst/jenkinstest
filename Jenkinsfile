pipeline {
    agent { docker 'python:3.5.1' }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                sh 'python --version'
            }
        }

        stage('Sanity check') {
            steps {
                input "Does the staging environment look ok?"
            }
        }

        stage("Deploy-Production") {
            steps {
                sh 'echo Deploy production'
            }
        }
    }
}
