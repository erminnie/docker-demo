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
	    stage('Build Image') {
		    steps {
         sh "docker build -t='erminnie/devopsgroup7demo-docker-webapp' ."
     }
 }
 stage('Push Image') {
     steps {
withCredentials([usernamePassword(credentialsId: 'docker', passwordVariable: 'pass', usernameVariable: 'user')]) {
             //sh
    sh "docker login --username=${user} --password=${pass}"
    sh "docker push erminnie/devopsgroup7demo-docker-webapp:latest"
}                           
     }
 }
                    }
              }
