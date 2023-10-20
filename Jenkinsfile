pipeline {
    agent any 
	environment {
		def scannerHome = tool 'sonar-scanner';
	
		
	
	}
    stages {
	  stage('SCM') {
		  steps {
		    checkout scm
		  }
	  }
	    

	  

	  stage('SAST with SonarQube') {
		  steps {
		    withSonarQubeEnv('SonarQube') {
		      sh "${scannerHome}/bin/sonar-scanner"
	    }
	    }
	  }


    
	    
	

	    

	    

	
	
	

	
    

        

    }
}
