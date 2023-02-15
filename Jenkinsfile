pipeline {
  agent any
//   environment {
//    PATH = "${PATH}" + ";c:\\Windows\\System32"
//  }
  stages {
    stage('version') {
      steps {
          bat 'python --version'
      }
    }
    stage('hello') {
      steps {
        bat 'python hello.py'
      }
    }
  }
}
