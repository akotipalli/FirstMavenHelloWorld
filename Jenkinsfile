pipeline {
    agent any 
    stages {
        stage('------------Clone Repo and clean it from Jenkinsfile-------------') { 
            steps {
               sh "mvn clean"
            }
        }
        stage('-------------Test from Jenkinsfile----------------') { 
            steps {
                sh "mvn test"
            }
        }
        stage('-------------Deploy from Jenkinsfile-----------------') { 
            steps {
               sh "mvn package"
            }
        }
    }
}
