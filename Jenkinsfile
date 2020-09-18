pipeline {
	    agent any { 
                  environment{
                                PATH="/usr/share/maven:$PATH"
		  		}
	      stages {
		        stage ('STAGE 1') {
		                      	steps {
				                              echo 'This is slaveforc node with STAGE 1'
				                              sh 'sleep 10'
		                             	}	
	          	                }
		        stage ('STAGE 2') {
			                    steps {
				                            echo 'This is slaveforjava with STAGE 2'
				                            sh "mvn clean package"
			                           }	
		                          }
		       
		      
		          }             
	    }
}
