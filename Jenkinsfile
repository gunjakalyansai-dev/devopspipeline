pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'to plan app'
      }
    }

    stage('code') {
      steps {
        echo 'full code for app'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'build the app '
          }
        }

        stage('test') {
          steps {
            echo 'test the app'
          }
        }

        stage('relese') {
          steps {
            echo 'release code'
          }
        }

        stage('deploy') {
          steps {
            echo 'deply app'
          }
        }

        stage('operate') {
          steps {
            echo 'operate the app'
          }
        }

      }
    }

  }
}