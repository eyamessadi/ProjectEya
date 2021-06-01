<<<<<<< HEAD:JenkinsFile
pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 5000:5000'
        }
    }
     
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        
    }
=======
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
>>>>>>> 6be6b2dfd321036b3625e44c0974e094bd639934:Jenkinsfile
}