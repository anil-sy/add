pipeline {
    agent {
		label 'ram'
	}

    tools {
       
        maven 'maven-3.9.4'
    }

    stages {
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
	    stage('print message') {
            steps {
               
                // Run Maven on a Unix agent.
		echo "done"
                sh "mvn clean install"

               
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
