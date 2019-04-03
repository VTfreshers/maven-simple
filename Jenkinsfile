pipeline {
	agent any
	stages {
	    stage ('build') {
			 steps {
			     echo "Building the sourcecode"
			 }
		}
		parallel {
			stage ('test: integration-&-quality') {
				 steps {
			     		echo "Testing is in progresss"
			 	}
			}
			stage ('test: functional') {
				 steps {
			     		echo "Functional test is going on"
			 		}
			}
			stage ('test: load-&-security') {
				  steps {
			      		echo "Load & Security"
			  		}
			}
		}
		stage ('approval') {
			  steps {
			      echo "Approval"
			  }
		}
		stage ('deploy:prod') {
			  steps {
			      echo "deploy"
			  }
		}
	}
}
