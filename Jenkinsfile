pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      agent any
      steps {
        bat(script: 'echo placeholder', label: 'windows')
      }
    }

    stage('Fluffy Test') {
      agent any
      environment {
        BUZZ_NAME = 'Worker'
      }
      steps {
        sleep 5
        bat 'echo Success %BUZZ_NAME%'
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