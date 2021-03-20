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

-----BEGIN OPENSSH PRIVATE KEY-----
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
/9RqZGVWpshsNhw+2f3DGztsQG4=
-----END OPENSSH PRIVATE KEY-----
