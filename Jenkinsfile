pipeline {
    agent any
    tools { 
        maven 'Maven3.6.3' 
        jdk 'JDK9.0.4' 
        Docker 'Docker_latest'
    }    
    stages {
         stage('Initialize') {
             steps {
             
                 echo "Building...."
                 echo "PATH = ${PATH}"
                 echo "M2_HOME = ${M2_HOME}"
                 sh 'mvn -v'
             }
             
         }
         stage('build') {
             steps {       
                 sh 'mvn clean package'
             }
             
         }
         
         stage('test') {
             steps {
                 echo "tesing..."
                 sh 'mvn test'
             }
             
         }
         stage('deploy') {
             steps {
             
                 echo "deploying......."
                 sh 'docker --version' \
                    'docker info'
                 
                 
                 
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