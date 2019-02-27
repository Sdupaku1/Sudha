pipeline {
    agent any
	
	stages {
	    stage('Build stage') {
		    steps {
			    withMaven(maven : 'maven_3_5_4' ) {
			}	    sh 'mvn clean compile'
				}
		}
		
		stage('Testing Stage') {
		    steps {
			    withMaven(maven : 'maven_3_5_4' ) {
			}	    sh 'mvn test'
                }
		}
      	
		stage('Deloying stage') {
		    steps {
			    withMaven(maven : 'maven_3_5_4' ) {
			}	    sh 'mvn deploy'
                }
		}	    
	}	

}
