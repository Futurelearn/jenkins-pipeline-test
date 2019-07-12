@Library('futurelearn') _

pipeline {
  agent { label 'ci' }
  stages {
    stage('Sleep') {
      steps {
        sh 'echo foo'
      }
    }
  }

  post {
    always {
      notify currentBuild.currentResult
    }
  }
}
