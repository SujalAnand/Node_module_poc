pipeline {
   agent any
    tools { 
        
        jdk 'jdk8' 
    }
          environment {
    
                PATH = "C:\\Users\\Administrator\\AppData\\Roaming\\npm\\:%PATH%"
            }
stages {
       stage('Deploy to Prod') {

          steps {
              echo "PATH is: %PATH%"
              bat 'newman --version'            
          }

       }
   }

}
