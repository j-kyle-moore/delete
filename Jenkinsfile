pipeline {
  agent none
  stages {
    stage('stage1') {
      parallel {
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

        stage('parallel 1') {
          agent {
            dockerfile {
              filename 'test'
            }

          }
          steps {
            echo 'hello'
          }
        }

        stage('parallel 2') {
          agent any
          steps {
            echo 'hola'
          }
        }

      }
    }

  }
}