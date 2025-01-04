pipeline {
    agent { label "ubuntu" }
    
    stages {
        stage('Hello') {
            steps {
                echo "Hello from Jenkinsfile"
            }
        }

        stage('for the staging branch') {
            when {
                branch "staging"
            }
            setps{
                sh '''Hello from staging'''
            }
        }
    }
}