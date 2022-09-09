pipeline {  
   agent none
   stages { 
       stage("Back-end") {
           agent {
               docker {image "maven:3.8.1-adoptopenjdk11"}
           }
           steps {
               sh "node --version"
           }    
       }
       stage("Front-end") {
           agent {
               docker {image "node:14-alpine"}
           }
           steps {
               sh "node --version"
           }
       }
   }
}
