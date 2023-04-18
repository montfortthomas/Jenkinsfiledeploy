pipeline{
 agent any
  stages {
    stage ('git checkout'){
      steps {
         git branch: 'main', credentialsId: '111', url: 'https://github.com/montfortthomas/Jenkinsfiledeploy.git'  
      }
     
     } 
    stage('pull code'){
      steps{
       sh " git pull --set-upstream origin main"
      
      }
     
    }
  
  }
 
}
