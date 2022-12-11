pipeline {
    agent any

    stages {

        stage('cleanWS') {
            steps {
                cleanWs()
            }
        }

        stage('clone git') {
            steps {
                git 'https://github.com/maharizi/Jenkins'
            }
        }
        stage('build') {
            steps {
                nodejs('Node8') {
                    sh "npm install"
                }
            }
        }
        stage('test') {
            steps {
                nodejs('Node8') {
                    sh "npm run test"
                }
    
            }

        }

    }
}
