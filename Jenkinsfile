pipeline {
  agent { label 'jenkins-agent-futurelearn' }

  stages {
    stage('Sleep') {
        steps {
          sshagent(credentials: ['futurelearn-ci-ssh']) {
            sh 'ssh git@github.com'
            sh 'sleep 300'
        }
      }
    }
  }
}
