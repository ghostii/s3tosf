pipeline
{
	agent any
	stages{
		stage('Build Application'){
		steps{
		bat 'mvn clean install'
		}
		}
	
		stage('MUnit Testing'){
		steps{
		bat 'mvn test'
		}
		}
		
		stage('Deploy Application to Cloudhub'){
		steps{
		bat 'mvn package deploy -DmuleDeploy'
		}
		}
	}
}