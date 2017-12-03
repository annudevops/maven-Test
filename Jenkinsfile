pipeline {
	{
	agent any
		tools { 
        maven 'M3' 
        jdk 'JAVA_HOME' 
    }
	
	stages {
		stage ('Compile Stage') {
			steps {
				{
					sh 'mvn clean compile'
				}
			}
		}

		stage ('Testing Stage') {
			steps {
				{
					sh 'mvn test'
				}
			}
		}
		stage ('Installing Stage') {
			steps {
				{
					sh 'mvn install'
				}
			}				
		}	
		
	}





