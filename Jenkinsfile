pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
    stage('pep8') {
      steps {
        sh 'flake8 --statistics'	    
      }
    }
    stage('test') {
      steps {
        sh 'python test.py'
      }   
    }
  }
}
