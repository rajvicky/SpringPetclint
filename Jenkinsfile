#!groovy
pipeline {
    agent none
    environment {
       env.PATH = env.PATH + ";c:\\Windows\\System32"
   }
   stages {    
    stage('Maven Install') {
      agent {         
       docker {          
         image 'maven:3.5.0'         
     }       
  }       
  steps {
       sh 'mvn clean install'
       }
     }
   }
 }
