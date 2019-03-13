pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'virtualenv -p python3 envname'
        sh 'source envname/bin/activate'
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
