node{
       
      stage('Checkout'){
         git 'https://github.com/ravismd/java-tomcat-maven-example.git'
       
      }   
       stage('Build'){
         //// Get maven home path and build
        
      }
     stage ('Test-JUnit'){
        
      }  
      stage('Deploy') {     
              sshagent(['ansible']) {
           
               sh 'scp -o StrictHostKeyChecking=no Jenkinsfile ansadmin@13.235.67.228:/home/ansadmin'
              }  
          }
         
     
      
 }
