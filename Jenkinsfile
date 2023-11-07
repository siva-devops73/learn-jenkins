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

            input {
               message "Should we continue?"
               ok "Yes, we should."
            }

            steps {
                echo 'Hello Siva'
            }
        }

        stage('Example Deploy') {
            when {
             branch 'production'
            }
            steps {
             echo 'Deploying'
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

// comment
