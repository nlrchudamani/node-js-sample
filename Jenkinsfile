pipeline {
  agent any
    
  tools {nodejs "nodejs"}
  BRANCH_NAME = "master"
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/nlrchudamani/node-js-sample.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
  }
}