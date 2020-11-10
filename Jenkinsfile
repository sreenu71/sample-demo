
pipeline {
    
    agent any
    def mvnHome = tool 'M3'
    
    stages {
        
        stage ('checkout') {
            steps {
                sh "git clone https://github.com/mitreid-connect/simple-web-app.git"
            }
        }
        
        stage ('build') {
            steps {
                
                sh "${mvnHome}/bin/mvn clean install -f simple-web-app"
            }
        }
    }
}
