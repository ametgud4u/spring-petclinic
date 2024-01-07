pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {
                sh 'cd /tmp'
                sh 'git clone https://github.com/ametgud4u/game-of-life.git'
            }
        }

        stage('Hello Neha') {
            steps {
                sh 'echo hello Neha'
            }
        }

        stage('Hello kedar') {
            steps {
                sh 'echo hello kedar'
            }
        }
    }
}
