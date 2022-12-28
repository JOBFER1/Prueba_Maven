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
	    	sh "cp -f /var/jenkins_home/workspace/target/Prueba_Maven.war /usr/local/tomcat/webapps"
	  	}
	}

  }
}