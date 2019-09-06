pipeline {
  agent { label 'ci' }
  stages {
    stage('Sleep') {
      when {
        changelog '^.*[publish].*$'
      }
      steps {
        sh 'sleep 10'
      }
    }
  }
}
