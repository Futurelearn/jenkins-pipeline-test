@Library('futurelearn@lm-fix-fresh-branch-bug') _

pipeline {
  agent any
  stages {
    stage('Foo') {
      steps {
        sh 'echo foo'
      }

      post {
        always {
          notify currentBuild.result
        }
      }
    }

  }
}
