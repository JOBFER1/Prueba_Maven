pipeline {
  agent any
  
  tools {
    maven 'Maven 3.8.6' 
  }

  stages {
    stage ('Build') {
      steps {
        sh 'mvn clean package'
      }
    }
    

    stage ('Deploy') {
    	steps {
	    	sh "docker cp /var/jenkins_home/workspace/Prueba_Maven/target/Prueba_Maven.war tomcat:/usr/local/tomcat/webapps"
	  	}
	}

  }
}