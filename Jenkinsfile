pipeline {
  agent { label 'jenkins-agent-futurelearn' }

  stages {
    stage('Sleep') {
      steps {
        sshagent(credentials: ['futurelearn-ci-ssh']) {
          sh 'mkdir ~/.ssh && ssh-keyscan github.com >> ~/.ssh/known_hosts'
          sh 'ssh git@github.com'
          sh 'sleep 300'
        }
      }
    }
  }
}
