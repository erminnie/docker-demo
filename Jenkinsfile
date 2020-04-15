pipeline {
    agent any
    
    tools {
          
        }

    stages {
          stage ("Nodejs") {
               steps {
                        nodejs('nodejs') {
                                   // some block
                                    echo "Nodejs configuration"
                                         }
                         }
                       }
			stage("Build") { 
            steps {
                sh 'npm install' 
                  }
                          }
                    }
              }
