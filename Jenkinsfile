pipeline{
    agent any
    	environment {
		notifyEmail ="rajibmahato885+jenkin@gmail.com"
	}
    tools{
        maven 'MAVEN_HOME'
    }
   //  triggers {
   //  	cron('0 06 * * *')
  	// }
    stages{
        stage("code checkout"){
            steps{
            bat "echo hello"
            }
        }   
        stage("code build"){
            steps{
            bat "mvn clean"
            }
        }
        stage("unit test"){
            steps{
            bat "mvn test"
            }
        }
    }
    post{
        success{
            bat "echo success"
            }
        }
}
