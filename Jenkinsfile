pipeline {
  agent any
  stages {
    stage('Source') {
      steps {
        git 'https://github.com/explore-jenkins/blue-ocean-demo.git'
      }
    }

    stage('Build') {
      steps {
        tool 'gradle7'
        sh 'gradle build'
      }
    }

  }
  environment {
    COMPLETED_MSG = 'Build done!'
  }
}