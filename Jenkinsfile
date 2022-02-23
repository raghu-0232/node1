pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/raghu-0232/node1.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'node index.js'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
