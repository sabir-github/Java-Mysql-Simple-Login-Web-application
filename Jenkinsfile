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
         echo 'Always'
      }
      success {
         echo 'Success'
      }
      failure {
         echo 'failure'
      }

      
  }
    
}