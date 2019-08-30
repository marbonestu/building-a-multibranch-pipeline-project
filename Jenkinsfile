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
        echo "start"
      }
    }
    stage ('Test') {
      steps {
        echo "test"
      }
      uiPipeline()
    }
  }
  post {
    always {
      echo "finished"
    }
  }
}
