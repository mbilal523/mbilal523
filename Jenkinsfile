pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'testing now'
      }
    }

    stage('Tuzz Tuzz') {
      parallel {
        stage('Tuzz Tuzz') {
          steps {
            echo 'UAT  - testing'
          }
        }

        stage('Test Final') {
          steps {
            archiveArtifacts(artifacts: 'target/*.jar ', fingerprint: true)
          }
        }

      }
    }

    stage('Cuzz Cuzz') {
      steps {
        echo 'Buzzing !'
      }
    }

  }
}