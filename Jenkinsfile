pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      parallel {
        stage('Fluffy Build') {
          agent any
          steps {
            bat(script: 'echo placeholder', label: 'windows')
          }
        }

        stage('Fluffy Temp Test') {
          steps {
            echo 'Hello Temp Test'
          }
        }

        stage('Fluffy Temp Test 2') {
          steps {
            echo 'Temp Test 2'
          }
        }

      }
    }

    stage('Fluffy Test') {
      agent any
      environment {
        BUZZ = 'Worker'
      }
      steps {
        sleep 5
        bat 'echo Success %BUZZ%'
      }
    }

    stage('Fluffy Deploy') {
      agent any
      steps {
        echo 'Placeholder'
      }
    }

  }
}