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
            steps{
                sh '''echo Hello from staging'''
            }
        }
    }
}