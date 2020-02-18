pipeline {
  agent { label 'jenkins-agent-futurelearn' }

  stages {
    stage('Sleep') {
      environment {
        SSH_KEY = credentials('futurelearn-ci-ssh')
      }
      steps {
        sh 'eval $(ssh-agent -s)'
        sh 'echo $SSH_KEY'
        sh 'ssh-add $SSH_KEY'
        sh 'ssh git@github.com'
        sh 'sleep 300'
      }
    }
  }
}
