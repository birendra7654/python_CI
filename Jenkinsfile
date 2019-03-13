pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'yum -y update'
        sh 'yum -y install python-pip'
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
