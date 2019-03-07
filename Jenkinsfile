pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo Build'
      }
    }
    stage('Unit Test') {
      parallel {
        stage('Unit Test') {
          steps {
            sh 'echo unit'
          }
        }
        stage('Performance') {
          steps {
            sh 'echo Perf'
            echo 'Performance'
          }
        }
      }
    }
    stage('Loadtest') {
      steps {
        echo 'Loadtest'
      }
    }
    stage('Frontend') {
      steps {
        echo 'Frontend'
      }
    }
  }
}