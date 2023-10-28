pipeline {

    agent { node { label 'workstation' } }

    environment {
      SSH = credentials('SSH')
    }

    options {
            ansiColor('xterm')
        }
        stages {
            stage('Build') {
                steps {
                    echo '\033[42m\033[97mWhite letters, green background\033[0m'
                }
            }
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
