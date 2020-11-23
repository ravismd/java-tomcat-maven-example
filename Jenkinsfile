node{
       
      stage('Checkout'){
         git 'https://github.com/ravismd/java-tomcat-maven-example.git'
       
      }   
      stage('Deploy') {     
            sshagent(['ansible']) {
               sh 'scp -o StrictHostKeyChecking=no target/tomcatdeploymnetdemo.war ansadmin@13.235.67.228:/opt/'
              
          }
         
     }
      
 }
