pipeline {
    
  environment {
    registry = "softwarece1/Eureka"
    //registryCredential = 'docker-creds'
    dockerImage = ''
  }
    
  agent any
    
  stages {
      
    stage('Cloning Git') {
      steps {
        git 'https://github.com/softwarece1/Eureka.git'
      }
    }
      
    stage('Building image') {
      steps{
        script {
          dockerImage = docker.build registry + ":$BUILD_NUMBER"
        }
     }
    }
  }
}

