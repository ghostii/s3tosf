pipeline
{
	agent any
	stages{
		stage('Build Application'){
		steps{
		bat 'cd s3tosf && mvn clean install'
		}
		}
		
		stage('Deploy Application to Cloudhub'){
		steps{
		bat 'cd s3tosf && mvn package deploy -DmuleDeploy'
		}
		}
	}
}
