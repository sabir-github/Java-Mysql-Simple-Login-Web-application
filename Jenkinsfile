pipeline {
    agent any
    tools { 
        maven 'Maven3.6.3' 
        jdk 'JDK9.0.4' 
    }    
    stages {
         stage('build') {
             steps {
             
                 echo "Building...."
                 echo "PATH = ${PATH}"
                 echo "M2_HOME = ${M2_HOME}"
                 maven clean
             }
             
         }
         stage('test') {
             steps {
              
                 
                 echo "tesing..."
                 echo "Test Successfull"
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