pipeline {
  agent any

  stages {
    stage('Create VENV') {
      steps {
          bat 'python -m venv env'
      }
    }
    stage('Activate VENV') {
      steps {
        bat 'env\\Scripts\\activate'
      }
    }
    stage('Install all requirements') {
      steps {
        bat 'pip install -r requirements.txt'
      }
    }
    stage('Run tests via Pytest') {
      steps {
        bat 'pytest --alluredir=allure_reports  calculator_tests/e2e_tests.py'
      }
    }
  }
}
