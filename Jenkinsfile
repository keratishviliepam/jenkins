pipeline {
  agent any
  stages {
    stage('git pull') {
      parallel {
        stage('print') {
          steps {
            echo 'Hello'
          }
        }

        stage('exec') {
          steps {
            sh 'echo "Jenkins"'
          }
        }

        stage('sleep') {
          steps {
            sleep 5
          }
        }

        stage('DevOpslab') {
          steps {
            echo 'This is Devops lab'
            sh 'echo "this is shell"'
          }
        }

      }
    }

    stage('Timestamps') {
      steps {
        timestamps()
      }
    }

  }
}