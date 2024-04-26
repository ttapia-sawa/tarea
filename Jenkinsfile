pipeline {
    agent any
    stages {
        stage('node pipeline') {
            agent {
                docker { image 'node:20.11.1-alpine3.19' }
            }
            stages {
                stage('install') {
                    steps {
                        sh 'npm install'
                    }

                }
                stage('test') {
                    steps {
                        sh 'npm install'
                    }

                }
                stage('build') {
                    steps {
                        sh 'npm build'
                    }

                }
            }
        }
    }
}
