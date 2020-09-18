pipeline {
	agent { label 'master' }  
                  stages {
		        stage ('STAGE 1') {
		                      	steps {
							build 'c-project-build'
				                             // echo 'This is slaveforc node with STAGE 1'
				                            //  sh 'sleep 10'
		                             	}	
	          	                }
		        stage ('STAGE 2') {
			                    steps {
						    	build 'java-project'
				                           // echo 'This is slaveforjava with STAGE 2'
				                           // sh "mvn clean package"
			                           }	
		                          }
		       
		      
		                      
	    }
}
