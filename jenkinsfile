pipeline { 
    agent any 
        stages { 
        
           stage('Build') {
            steps {
                sh 'mvn clean install'
                //archiveArtifacts artifacts: '/target/window.jar', fingerprint: true 
                }
            }
            
        }
    }
