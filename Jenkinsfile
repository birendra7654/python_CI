pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'sudo pip install -r requirements.txt'
      }
    }
    stage('pep8') {
      steps {
        sh 'sudo flake8 --statistics'	    
      }
    }
    stage('test') {
      steps {
        sh 'sudo python test.py'
      }   
    }
  }
}
