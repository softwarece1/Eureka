pipeline { 
    environment {
    registry = "softwarece1/Eureka"
   dockerImage = ''
  }
    
    
    agent any 
    
        stages { 
        
           stage('Compile') {
            steps {
                bat 'mvn compile'
                }
            }
            
           stage('Test') {
            steps {
                bat 'mvn test'
                }
            }
            
           stage('Package') {
            steps {
                bat 'mvn package'
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


