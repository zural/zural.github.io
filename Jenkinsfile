pipeline {
  agent any
  stages {
    stage('Develop') {
      parallel {
        stage('Develop') {
          steps {
            bat(script: 'Develop', label: 'Develop')
          }
        }
        stage('Step') {
          steps {
            echo 'Step'
          }
        }
      }
    }
    stage('Qa') {
      steps {
        echo 'QA'
      }
    }
  }
}