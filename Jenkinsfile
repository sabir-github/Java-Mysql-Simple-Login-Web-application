pipeline {
    agent any
    stages {
         stage('build') {
             steps {
             
                 echo "Build successfull"
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
         echo 'Always3---fk'
      }
      success {
         echo 'Success3'
      }
      failure {
         echo 'failure3'
      }

      
  }
    
}