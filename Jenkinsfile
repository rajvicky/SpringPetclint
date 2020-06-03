#!groovy
pipeline {
    environment {
    PATH = "C:\\WINDOWS\\SYSTEM32;C:\\Program Files\\Docker Toolbox;C:\\Program Files\\Git\\bin\\sh.exe"
}
    agent any 
    stages {
        
          stage("Test sh script in container") {
           steps {
                sh 'printenv'
            }
        }
    }
}
