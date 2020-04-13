node {
   
   def mvn = tool (name: 'Maven-3.6.3', type: 'maven') + '/bin/mvn'
             
   
  stage('Checkout') {
       git branch: 'master', credentialsId: 'd1308b62-5515-4b17-a89b-2452cb3c4cd5', url: 'http://adept-gitsource.sonata-software.com/Open_Source_Competency/catalog-service.git'
   }
   
   
   stage('Mvn Package'){
	   // Build using maven
	   
	  // sh "${mvn} clean install -DskipTests"
	  bat "${mvn} clean package deploy"
   }
   
   
   
}