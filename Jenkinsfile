node{
       
      stage('Checkout'){
         git 'https://github.com/ravismd/java-tomcat-maven-example.git'
       
      }  
      stage('Build'){
         //// Get maven home path and build
        sh "mvn clean package -Dmaven.test.skip=true"
      }
     stage ('Test-JUnit'){
         sh "mvn test"
      } 
    
      stage('Deploy') {     
            sshagent(['Tomcat-jenkins']) {
               sh 'scp -o StrictHostKeyChecking=no target/tomcatdeploymnetdemo.war ansadmin@13.235.67.228:/opt/'
              
          }
         
     }
      
 }
