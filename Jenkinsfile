pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        withEnv(['PATH+EXTRA=/usr/sbin:/usr/bin:/sbin:/bin']) {
          sh 'python --version'
        }
      }
    }
    stage('hello') {
      steps {
        sh 'python hello.py'
      }
    }
  }
}
