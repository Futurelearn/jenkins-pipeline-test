@Library('futurelearn@lm-reduce-parameters') _

pipeline {
  agent any
  stages {
    stage('Foo') {
      steps {
        sh 'echo foo'
      }

      post { always { notify '#notifications' } }
    }

  }
}
