pipeline{
	agent any
	stages{
		stage('Build Application'){
		steps{
			bat 'mvn clean install'
		}}
		stage('Deploy application to Mulesoft Cloudhub'){
		steps{
			bat 'mvn clean install'
		}}
		stage('Perform Regresssion testing'){
			steps{
			bat 'newman run C:\\NewMan\\WorldTimeZone.postman_collection.json --disable-unicode'
		}}
	}
	
}