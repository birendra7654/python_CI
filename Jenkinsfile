pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'sudo apt update'
        sh 'sudo apt install python3-pip'
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
