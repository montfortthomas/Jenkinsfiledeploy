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
   
   stage('deploy'){
    steps{
          sshagent(['112']) {
         
               sh "cd /var/lib/jenkins/workspace/Jenkinsfile-deploy"
               sh "ls"
               
           
           //sh "mv"
             //  sh """
               //ssh -tt "ec2-user@43.204.32.91"
               //sh "ls"
               
              // """//
               
           //sh "mv .* ec2user-@43.204.32.91:/var/www/html/ "//
           
}
    
    }
   }
   
   
  
  }
 
}
