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
         echo 'Always2'
      }
      success {
         echo 'Success2'
      }
      failure {
         echo 'failure2'
      }

      
  }
    
}