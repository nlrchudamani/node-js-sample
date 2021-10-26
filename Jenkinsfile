pipeline {
  agent any
    
  tools {nodejs "node"}
    
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
        sh 'node test'
      }
    }
  }
}