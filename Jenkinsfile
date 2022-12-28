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
	    	sh "cp -f /target_jenkins/jobs/Prueba_Maven/workspace/target/Prueba_Maven.war /usr/local/tomcat/webapps"
	  	}
	}

  }
}