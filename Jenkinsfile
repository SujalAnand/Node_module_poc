pipeline {
  agent any
  tools { 
        maven 'maven-3.6.3'
        jdk 'jdk8' 
  }
  environment {
		 PATH = "C:\\Users\\Administrator\\AppData\\Roaming\\npm\\:%PATH%"
      }

  stages {
    stage ('Initialize') {
            steps {
                bat '''
                    echo "PATH = %PATH%"
                    echo "M2_HOME = %M2_HOME%"
                ''' 
       }
    }
    stage('Regression Testing') {
      steps {
	    echo "~~~~~~~Running Postman Scripts~~~~~~~~~"
            bat 'newman run "C:\\Users\\Administrator\\Desktop\\Postman_Collection\\CI-CD-GetFlights-Jenkins.postman_collection.json"  -r htmlextra --reporter-htmlextra-export "C:\\Users\\Administrator\\Desktop\\Postman_Collection" --reporter-htmlextra-darkTheme'
      }
    }
	

  }
}
