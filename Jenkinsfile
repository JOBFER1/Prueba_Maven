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
	    	bat "powershell Copy-Item C:\AA-Subvención autónomos Cantabria\Cursos CLEFormacion_Elena Hervas\Ecosistemas Desarrollo\workspace\Jenkis_Docker_Home\workspace\Prueba_Maven\target\Prueba_Maven.war -Destination C:\AA-Subvención autónomos Cantabria\Cursos CLEFormacion_Elena Hervas\Ecosistemas Desarrollo\workspace\Jenkis_Docker_Home\tomcat\webapps"
	  	}
	}

  }
}