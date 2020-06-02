#!groovy
pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        }
          stage("Test sh script in container") {
            steps {
              sh label: 'Echo "Hello World...', script: 'echo "Hello World!"'
            }
        }
    }
}
