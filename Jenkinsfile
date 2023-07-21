pipeline{
    agent any
    	environment {
		notifyEmail ="rajibmahato885+jenkin@gmail.com"
	}
    tools{
        maven 'MAVEN_HOME'
    }

    stages{
        stage("Framework checkout"){
            steps{
            bat "echo hello"
            }
        }   
        stage("Framework build"){
            steps{
            bat "mvn clean"
            }
        }
        stage("Framework test"){
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
