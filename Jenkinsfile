pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is development'
      }
    }

    stage('test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build'
          }
        }

        stage('fixes') {
          steps {
            echo 'this is fix'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate'
          }
        }

        stage('prod') {
          steps {
            echo 'this is prod'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deployment'
          }
        }

      }
    }

  }
}