pipeline {

    agent { node { label 'workstation' } }

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
      }
    }
}
