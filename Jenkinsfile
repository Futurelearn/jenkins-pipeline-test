@Library('futurelearn@lm-reduce-parameters') _

pipeline {
  agent any
  stages {
    stage('Foo') {
      steps {
        sh 'false'
      }

      post {
        always { notify '#notifications' }
      }
    }

  }
}
