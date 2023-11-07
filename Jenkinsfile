pipeline {

    agent { node { label 'workstation' } }

    environment {
      SSH = credentials('SSH')
    }

    options {
            ansiColor('xterm')
        }

    triggers { pollSCM('H/2 * * * *') }

     parameters {
        string(name: 'APP_INPUT', defaultValue: '', description: 'Just Input')
     }


    stages {
        stage('Hello-1') {
            steps {
                echo 'Hello Siva'
            }
        }
    }

    post {
      always {
         echo 'siva kumar good morning'
         sh 'env'
      }
    }
}
