pipeline {

    agent { node { label 'workstation' } }

    environment {
      SSH = credentials('SSH')
    }

    options {
            ansiColor('xterm')
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
