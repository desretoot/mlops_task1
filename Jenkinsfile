pipeline {
  agent any
  stages {
    stage('install') {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }
    stage('data_creation') {
      steps {
        sh 'python3 data_creation.py'
      }
    }
    stage('model_preprocessing') {
      steps {
        sh 'python3 model_preprocessing.py'
      }
    }
    stage('model_preparation') {
      steps {
        sh 'python3 model_preparation.py'
      }
    }
    stage('model_testing') {
      steps {
        sh 'python3 model_testing.py'
      }
    }
  }
}