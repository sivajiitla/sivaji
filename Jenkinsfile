pipeline {
    agent any
    stages {
        stage ('Build Servlet Project') {
		tools {
       			 maven 'Maven 3.6.1'
    			}
            steps {
                /*For windows machine */
               sh  'mvn clean package'

                /*For Mac & Linux machine */
               // sh  'mvn clean package'
            }

            post{
                success{
                    echo 'Now Archiving ....'

                    archiveArtifacts artifacts : '**/*.war'
                }
            }
        }
	}
}
