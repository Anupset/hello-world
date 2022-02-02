pipeline{
  agent any

   stages{
      stage ('compile stage') {
        steps {
          withMaven(maven: 'maven-3.8.4'){
               sh 'mvn clean compile'
             }
        }
   }
   stage ('testing stage') {
        steps {
          withMaven(maven: 'maven-3.8.4'){
               sh 'mvn test'
             }
        }
   }
   stage ('deployment stage') {
        steps {
          withMaven(maven: 'maven-3.8.4'){
               sh 'mvn deploy'
             }
        }
   }
