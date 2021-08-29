pipeline{
  agent any
   tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven3"
    }
  stages{
       stage('get SCM'){
	       steps{
	         git credentialsId: 'Github_credentials', url: 'https://github.com/vijayammanagi1234/spring3-mvc-maven-xml-hello-world.git'
	        }
	    }
		
		stage('gbuild'){
	       steps{
	         sh "mvn packages"
	        }
	    }
}
}
