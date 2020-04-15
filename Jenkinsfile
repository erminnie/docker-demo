pipeline {
    agent any
    
    tools {
          nodejs 'nodejs'
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
