pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i want to Build'
      }
    }

    stage('test') {
      steps {
        echo 'i want to test'
      }
    }

    stage('stag') {
      parallel {
        stage('stag') {
          steps {
            echo 'i want to stag'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'i want to operate'
          }
        }

      }
    }

  }
}