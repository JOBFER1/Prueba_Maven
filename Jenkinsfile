pipeline {
  agent any
  
  tools {
    maven 'Maven 3.8.6' 
  }

  stages {
    stage ('Build') {
      steps {
        sh 'mvn --version'
      }
    }
    

    stage ('Deploy') {
    	steps {
	    	"docker cp jenkins:/var/jenkins_home/workspace/Prueba_Maven/target/Prueba_Maven.war tomcat:/usr/local/tomcat/webapps"
	  	}
	}

  }
}