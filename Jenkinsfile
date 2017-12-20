node('master') {
  
   stage 'Git Checkout'
     git 'https://github.com/arghya1990/jenkinsPipelineBuildTestDeploy.git'
     echo 'checkout done'

  
  stage('Maven Build'){    
    echo 'Maven Project Compile'      
    maven 'clean install' 
           
    junit 'target/surefire-reports/**/*.xml'     
      
  }
  stage 'Deploy'  
  echo 'Deploying Docker Image'
  
   stage 'Testing'   
   echo 'Reporting Getting Creating'
  
   stage 'Job Status Report'    
   echo 'Sending Notification'
}
