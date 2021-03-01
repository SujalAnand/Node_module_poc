pipeline {
   agent any
    tools { 
        maven 'maven'
        jdk 'jdk8' 
    }
          environment {
                ANYPOINT_CREDENTIALS = credentials('anypoint.credentials')
                PATH = "C:\\Users\\Administrator\\AppData\\Roaming\\npm\\:%PATH%"
            }

       stage('Deploy to Prod') {

          steps {
              echo "PATH is: %PATH%"
              echo "Deploying $applicationName to Prod..."
              bat 'newman --version'            
          }

       }
   }
