pipeline {  
  agent {
    docker { image "node:14-alpine" }
  }
  stages { 
    stage("Prebuild") {
      steps {
        echo "Prebuild"
        sh "node --version"
      }    
    }
    stage("Test") {
      steps {
        echo "test"
      }
    }
    stage("Postbuild") {
      steps {
        echo "Postbuild"
        sh "node --version"
      }
    }
  }
}
