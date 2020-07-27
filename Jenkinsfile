pipeline
 {
  agent any
   {
   stages{    
    stage('Build Application'){
     steps{
      bat 'mvn clean  install'
      }
     }
     
    stage('Deploy Application to MuleSoft CloudHub'){
     steps{
     bat 'mvn package deploy -DmuleDeploy'
     }
     }
     
     
    stage('Perform Regression Testing'){
      steps{
       bat 'C:\\Users\\vreddygari\\AppData\\Roaming\\npm\\newman run D:\\newman\\WorldTimeZone-Collections.postman_collection.json --disable-unicode
       }
     }
     
     
     
    }
   }
 }