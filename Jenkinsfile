pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build1') {
          steps {
            echo 'Build 1'
          }
        }

        stage('Build2') {
          steps {
            echo 'Build 2'
          }
        }

      }
    }

    stage('Deploy') {
      parallel {
        stage('Deploy1') {
          steps {
            echo 'Deploy 1'
          }
        }

        stage('Deploy2') {
          steps {
            echo 'Deploy 2'
          }
        }

      }
    }

    stage('SmokeTest') {
      parallel {
        stage('SmokeTest1') {
          steps {
            echo 'Smoke Test 1'
          }
        }

        stage('SmokeTest2') {
          steps {
            echo 'Smoke Test 2'
          }
        }

        stage('') {
          steps {
            build 'testjob'
          }
        }

      }
    }

  }
}