currentBuild.displayName="Hello-World-Project-#"+currentBuild.number

pipeline {
   agent any

   stages {
      stage("Git Checkout") {
         steps {
          git 'https://github.com/tusharheda08/onewebapp.git/'
           // git 'https://github.com/tusharheda08/onewebapp'
            
         }
      }
       stage("Maven Build") {
         steps {
            // def mvnHome = tool name: 'Maven', type: 'maven'
           //  sh "${mvnHome}/bin/mvn package"
            
            sh script: 'mvn -f webapp-one/pom.xml'
            
            
         }
      } 
       
    }
 }
      
   

