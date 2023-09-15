pipeline {
    agent {
		label 'ram'
	}

    tools {
       
        maven 'maven-3.9.4'
    }

    stages {
		stage('Scm-checkout') {
			steps {
				
				git 'https://github.com/anil-sy/add.git'
				}
			}
			
		 stage('compile') {
            steps {
               
                // Run Maven on a Unix agent.
                sh "mvn compile"

               
            }

          
        }
		stage('Test') {
            steps {
               
                // Run Maven on a Unix agent.
                sh "mvn test"

               
            }

          
        }
		stage('package') {
            steps {
               
                // Run Maven on a Unix agent.
                sh "mvn package"

               
            }

          
        }
    }
}
