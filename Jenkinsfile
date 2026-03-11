pipeline {
    agent any
    stages {
        stage('Fetching File') {
            steps {
               git branch:'master',url:'https://github.com/Yash-Singh0408/jenkins-demo.git'
            }}
        stage('Build') {
            steps {
                echo 'Building Project'
                bat 'javac Hello.java'
            }}
        stage('Execute') {
            steps {
                echo 'Executing Program'
                bat 'java Hello'
            }}
        stage('Deploy') {
            steps {
                echo 'Deploying Project'
            }}}
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
echo 'Pipeline failed'
}}}
