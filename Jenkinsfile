pipeline {
    agent any
   
    
    environment {
       
        NEXUS_VERSION = "nexus3"
        NEXUS_PROTOCOL = "http"
        NEXUS_URL = "http://localhost:8083"
        NEXUS_REPOSITORY = "java-app"
        NEXUS_CREDENTIAL_ID = "NEXUS_CRED"
    }
    stages {
        stage("Clone code from GitHub") {
            steps {
                script {
                    git branch: 'main', credentialsId: 'githubwithpassword', url: 'https://github.com/abhinavbhardwaj0732/jenkins-nexus-1';
                }
            }
        }
