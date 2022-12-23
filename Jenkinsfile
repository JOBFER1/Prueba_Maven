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
	    	sh "sudo cp -f -S target/Prueba_Maven.war /opt/Innovecture/apache-tomcat-10.0.27/webapps"
	  	}
	}

  }
}