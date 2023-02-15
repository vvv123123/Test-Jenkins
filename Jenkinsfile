pipeline {
  agent any
  environment {
     PATH = "C:\\Users\\volodymyr.sydor\\AppData\\Local\\Programs\\Python\\Python310;c:\\Windows\\System32"
 }
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
