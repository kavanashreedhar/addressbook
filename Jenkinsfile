pipeline {
    agent any
    stages {
         stage('Listing') {
            steps { 
                echo 'Cloning addressbook git-repo'
            }
        }
        stage('Compile') {
            steps { 
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps { 
                sh 'mvn test'
            }
        }
        stage('package') {
            steps { 
                sh 'mvn package'
            }
        }
    }
}
