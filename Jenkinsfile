pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'ping -c 2 localhost'
      }
    }
    stage('Test') {
      parallel {
        stage('Test_1') {
          steps {
            sh 'ping -c 3 localhost'
          }
        }
        stage('Test_2') {
          steps {
            sh 'ping -c 5 localhost'
          }
        }
        stage('Test_3') {
          steps {
            sh 'sdsfdsfdsdfdsf'
          }
        }
        stage('Test_4') {
          steps {
            sh 'ping -c 3 localhost'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'ping -c 4 localhost'
      }
    }
  }
}