#!groovy
pipeline {
    agent none
   stages {   
      stage('build') {
            steps {
                sh 'python --version'
            }
        }  
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