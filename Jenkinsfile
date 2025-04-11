pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }
        stage('Read hello.txt') {
            steps {
                script {
                    def content = readFile('hello.txt')
                    echo "${content}"
                }
            }
        }
    }
}
