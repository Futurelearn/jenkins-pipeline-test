pipeline {
  agent { ecs { inheritFrom 'jenkins-agent-futurelearn' } }

  stages {
    stage('Sleep') {
      steps {
        sh 'sleep 300'
      }
    }
  }
}
