pipeline {
	agent none 
                  stages {
			  stage ('make and mavan') {
				  parallel{
					  
			  stage ('STAGE 1') { agent {label 'node'}
		                      	steps {
							git 'https://github.com/sharathpvs123/repo1.git'
							sh 'make'
		                             	}	
	          	                }
			  stage ('STAGE 2') { agent {label 'node2'}
			                    steps {
						    	git 'https://github.com/sharathpvs123/hello-world.git'
						    	sh 'mvn clean install'
			                           }	
		                          }
				  
				  
				  
				  }
				  
				  
			  }
		      
		                      
	    }
}
