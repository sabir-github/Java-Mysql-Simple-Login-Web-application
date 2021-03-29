pipeline {
    agent any
    tools { 
        maven 'Maven 3.3.9' 
        jdk 'jdk8' 
    }    
    stages {
         stage('build') {
             steps {
             
                 echo "Build successfull"
                 echo "PATH = ${PATH}"
                 echo "M2_HOME = ${M2_HOME}"
             }
             
         }
         stage('test') {
             steps {
              
                 echo "test successfull"
             }
             
         }
         stage('deploy') {
             steps {
             
                 echo "deploy successfull"
             }
             
         }
         
    }
  post {
      always {
         echo 'Always3--'
      }
      success {
         echo 'Success3'
      }
      failure {
         echo 'failure3'
      }

      
  }
    
}