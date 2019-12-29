pipeline {
    agent none
    stages {
        stage('Back-end') {
            agent {
                docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                docker { image 'node:7-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
        stage('tomas73') {
            agent {
                docker { image 'tomas73/cheers2019' }
            }
            steps {
                sh 'bash --version'
            }
        }

    }
}
