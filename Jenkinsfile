pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'testing now'
      }
    }

    stage('Tuzz Tuzz') {
      steps {
        archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
      }
    }

  }
}