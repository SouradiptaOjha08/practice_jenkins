pipeline{
	agent any 
	tools
	{
		maven 'MAVEN_HOME'
	}
	stages{
		stage('Welcome stage')
		{
			steps
			{
				echo 'Welcome stage'
			}
		}
		stage ('Clean stage') {
			steps
			{
				sh 'mvn clean'
			}
			
		}
		stage ('Build stage'){
			steps {
				sh 'mvn install'
			}
		}
		stage ('Success stage'){
			steps {
				echo 'Success stage completed'
			}
		}
	}
}