pipeline {  
   agent { dockerfile true }
   stages { 
      stage("Prebuild") {
        steps {
           echo "prebuild"
           sh "node --version"
           sh "svn --version"
        }    
      }
      stage("Test") {
        steps {
           echo "test"
        }    
      }
      stage("Postbuild") {
        steps {
           echo "postbuild"
           sh "node --version"
        }    
      }
   }
}
