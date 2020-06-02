#!groovy
pipeline {
    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32;C:\\Program Files\\Docker Toolbox;C:\\Program Files\\Git\\bin\\sh.exe"
}
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
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
          stage("Test sh script in container") {
            steps {
              sh label: 'Echo "Hello World...', script: 'echo "Hello World!"'
            }
        }
    }
}
