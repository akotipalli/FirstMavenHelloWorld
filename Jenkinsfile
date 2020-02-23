pipeline {
    agent any 
    stages {
        stage('------------Clone Repo and clean it from Jenkinsfile-------------') { 
            steps {
                sh "rm -rf FirstMavenHelloWorld"
               sh "git clone https://github.com/akotipalli/FirstMavenHelloWorld.git"
               sh "mvn clean -f FirstMavenHelloWorld"
            }
        }
        stage('-------------Test from Jenkinsfile----------------') { 
            steps {
                sh "mvn test -f FirstMavenHelloWorld"
            }
        }
        stage('-------------Deploy from Jenkinsfile-----------------') { 
            steps {
               sh "mvn package -f FirstMavenHelloWorld"
            }
        }
    }
}
