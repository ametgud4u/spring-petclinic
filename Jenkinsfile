pipeline {
        agent {
        label 'knode1'
         }
        stages {
          stage("SCM") {
            steps {
             sh "echo SCM"
              }
            }
          stage("build & SonarQube analysis") {
            steps {
              sh "echo SonarQube analysis"
              }
            }
		  stage("HOSTNAME") {
            steps {
             sh "hostname"
              }
            }
        }
   }
