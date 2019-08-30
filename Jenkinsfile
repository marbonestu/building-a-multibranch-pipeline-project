@Library('pui-pipeline') _

pipeline {
  agent {
    // Use docker container
    docker {
      image 'node:latest'
    }
  }
  stages {
    stage ('Start') {
      steps {
        // send build started notifications
      }
    }
    uiPipeline()
    stage ('Test') {
      steps {
        // run tests with coverage

      }
    }
  }
  post {
    always {
      echo "finished"
    }
  }
}
