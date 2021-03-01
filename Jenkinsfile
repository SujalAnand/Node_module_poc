pipeline {
   agent any
    tools { 
        
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
   }

}
