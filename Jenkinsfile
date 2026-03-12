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
                   allowmissing:true,
                   alwaysLinktoLastBuild:false,
                   keepAll:false,
                   reportDir:'.',
                   reportFiles:'first.html',
                   reportName:"Name hai ye"
               ])
               }
            }
       }
}
