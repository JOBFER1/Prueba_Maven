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
    		docker exec container bash -c 'hostname -I ; wget –URI root@172.21.0.3://var/jenkins_home/workspace/Prueba_Maven.* -UseBasicParsing'
	  	}
	} 

  }
}