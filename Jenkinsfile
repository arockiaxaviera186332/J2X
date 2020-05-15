pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('step1') {
          steps {
            echo 'Build'
            echo 'Build 1'
          }
        }

        stage('step2') {
          steps {
            echo 'build1'
          }
        }

      }
    }

    stage('Deploy1') {
      parallel {
        stage('Deploy1') {
          steps {
            echo 'Deploy 1'
          }
        }

        stage('Deploy 2') {
          steps {
            echo 'Deploy 2'
          }
        }

      }
    }

    stage('Test 1') {
      parallel {
        stage('Test 1') {
          steps {
            echo 'test'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test'
          }
        }

      }
    }

  }
}