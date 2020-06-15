properties([parameters([choice(choices: 'master\nfeature\nhotfix', description: 'Select the branch', name: 'branch')])])

pipeline {
    agent {label 'master'}
    stages {
        stage('Source'){
            steps {
                git url:'https://github.com/ametgud4u/spring-petclinic.git', branch: "${params.branch}" 
            }
        }
        stage('Package'){
            steps {
                sh 'mvn package'
            }
        }
    }
}