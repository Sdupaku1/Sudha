pipeline {
    agent any
	
	stages {
	    stage('Build stage') {
		    steps {
			    withMaven(maven : 'maven_3_6_0' )
			}	sh 'mvn clean compile'
		}
		
		stage('Testing Stage') {
		    steps {
			    withMaven(maven : 'maven_3_6_0' )
			}	sh 'mvn test'
		}
		
		stage('Deloying stage') {
		    steps {
			    withMaven(maven : 'maven_3_6_0' )
			}	sh 'mvn deploy'
		}	    
	}	

}