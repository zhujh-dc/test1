pipeline {
  agent any
  stages {
    stage('compile') {
      parallel {
        stage('compile') {
          steps {
            sh 'echo abc'
          }
        }

        stage('compile1') {
          steps {
            sh 'echo compile1'
          }
        }

        stage('') {
          steps {
            cleanWs(cleanWhenAborted: true, cleanWhenFailure: true)
          }
        }

      }
    }

    stage('package') {
      steps {
        echo 'abc'
      }
    }

  }
  environment {
    a = '123'
  }
}