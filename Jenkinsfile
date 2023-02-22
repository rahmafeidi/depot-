node {

  try {
  
  stage('Code Checkout') { 
      // Get some code from a GitHub repository
      git 'https://github.com/rahmafeidi/depot-.git'
  
   }
   
   stage('Unit Test') { 
       withEnv(['PATH+EXTRA=/opt/apache-maven-3.6.3/bin']) {
      // Get some code from a GitHub repository
        sh 'mvn clean compile'
        sh 'mvn test'
        }
   }
   
     

} catch(e) {
	echo "Caught some exception"
	
  }  finally {
	echo "Finally Block"
	
}
    
}
