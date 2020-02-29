pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            echo 'Hello world!'
            sleep 10
            mail(subject: 'Build completed', body: 'The build has been completed', to: 'thomas.briot82@gmail.com')
          }
        }

        stage('Stage 1.1') {
          steps {
            echo 'Stage 1.1 !'
          }
        }

      }
    }

    stage('Stage 2') {
      steps {
        echo 'Hello world Github webhook !!!'
      }
    }

  }
}