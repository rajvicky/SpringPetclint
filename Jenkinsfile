#!groovy
pipeline {
    agent none
    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32;C:\\Program Files\\Docker Toolbox"
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
