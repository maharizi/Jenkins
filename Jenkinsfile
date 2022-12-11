pipeline {
    agent any

    stages {
        stage('git clone & build') {
            steps {
                parallel(
                    a: {
                        echo "This is branch a"
                    },
                    b: {
                        echo "This is branch b"
                    }
                )
            }
        }
        stage('test') {
            steps {
                echo 'test'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploy'
            }
        }
    }
}
