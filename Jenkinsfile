pipeline {
    agent any
    stages {
        stage("Checkout"){
              steps{
                git "https://github.com/Yash-Singh0408/jenkins-demo.git"   
               }
            }

         stage("Publish"){
              steps{
               publishHTML([
                   allowMissing:true,
                   alwaysLinkToLastBuild:false,
                   keepAll:false,
                   reportDir:'.',
                   reportFiles:'first.html',
                   reportName:"Name hai ye"
               ])
               }
            }
       }
}
