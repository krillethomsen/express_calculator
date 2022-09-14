pipeline {  
   agent any
   stages { 
      stage("Prebuild") {
        steps {
           sh "npm install"
        }    
      }
      stage("Unit test") {
        steps {
           sh "npm run test-unit"
        }    
      }
      stage("Integration test") {
        steps {
           when{
             anyOf{
               branch "develop";
               branch "main"
             }
           }
           sh "npm run test-integration"
        }    
      }
   }
}
