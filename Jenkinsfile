pipeline {
  agent any
    
  tools {nodejs "NodeJS"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/eyamessadi/ProjectEya.git'
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