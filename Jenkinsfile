pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/brianmarete/node-todo'
      }
    }
        // Comment
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }

    // Comment
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}