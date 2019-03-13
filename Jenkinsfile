pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'sudo yum -y update'
        sh 'sudo yum -y install python-pip'
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
        sh 'sudo python test_calculator.py'
      }   
    }
  }
}
