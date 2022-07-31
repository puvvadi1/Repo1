pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('hi') {
            steps {
                echo 'Welcome to job1'
            }
        }
        parallel {
            stage('parallel1') {
                steps {
                    timeout 5
                    echo 'Welcome to parallel1'
                }
            }
            stage('parallel2') {
                steps {
                    echo 'Welcome to parallel2'
                }
            }
        }
    }
}

