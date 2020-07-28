
pipeline
 {
  agent any
   stages{
   stage('Build Application'){
   step{
   bat 'mvn clean install'
   }
   }
   
   stage('Munit Test Application'){
   step{
   bat 'mvn test'
   }
   }
   
   stage('Deploy application to CloudHub'){
   step{
   bat 'mvn package deploy -DmuleDeploy'
   }
   }
   
   stage('Perform Regression testing'){
   step{
   bat 'C:\\Users\\vreddygari\\AppData\\Roaming\\npm\\newman run D:\\newman\\WorldTimeZone-Collections.postman_collection.json --disable-unicode'
   }
   }
   
   
   }
 }