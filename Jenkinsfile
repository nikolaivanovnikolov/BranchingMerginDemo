#!groovy

/**
 * This is the pipeline for developing BWC.
 *
 * You can find the shared library 'pipeline' code here:
 **/

pipeline {
  agent { label 'master' }
  stages {
    stage('Build') {
      agent { label 'master' }
      steps {
        echo 'Step: Building...'
      }
    }
    stage('Test') {
      agent { label 'master' }
      steps {
          echo 'Step: Testing...'
      }
    }
    stage('Deploy') {
      agent { label 'master' }
      steps {
        echo 'Step: Deploying...'
        sh "chmod +x HelloWorld.sh "
        sh ". / HelloWorld.sh "
      }
    }
  }
}
