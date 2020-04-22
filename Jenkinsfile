pipeline {
    agent any
   stages {
       stage('Compile stage')
       steps{
           withMaven(maven : 'maven:3.6.3') {
               sh 'Maven clean compile'
           }
       }
   }
    stages {
       stage('Testing Stage')
       steps{
           withMaven(maven : 'maven:3.6.3') {
               sh 'Maven Test'
           }
       }
   }
     stages {
       stage('Deployment Stage')
       steps{
           withMaven(maven : 'maven:3.6.3') {
               sh 'Maven Deploy'
           }
       }
   }
    
}
