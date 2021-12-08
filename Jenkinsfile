pipeline {
  agent none
  stages {
    stage('stage1') {
      agent {
        node {
          label 'default'
        }

      }
      steps {
        echo 'hi ryan'
      }
    }

  }
}