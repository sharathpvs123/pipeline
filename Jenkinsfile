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
					stage ('STAGE 3') {
			agent { label 'master' }
			steps {
				echo 'This is slaveforc with STAGE 3'
				sh 'sleep 10'
			}	
		}
		stage ('STAGE 4') {
			agent { label 'slaveforc' }
			steps {
				echo 'This is master with STAGE 4'
				sh 'sleep 10'
			}	
		}  
				  
				  
				  }
				  
				  
			  }
		      
		                      
	    }
}
