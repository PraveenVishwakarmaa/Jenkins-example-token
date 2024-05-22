pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test stsge'
          }
        }

        stage('Test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}