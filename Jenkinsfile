pipeline {
    agent {label 'Nodejs_slave1'}
    stages {
        stage('Back-end') {
            agent {
                /usr/bin/docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Front-end') {
            agent {
                /usr/bin/docker { image 'node:7-alpine' }
            }
            steps {
                sh 'node --version'
            }
        }
    }
}
