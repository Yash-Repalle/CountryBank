pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/Yash-Repalle/CountryBank.git'
            }
        }
        
        // stage('Code Compile') {
        //     steps {
        //          sh 'mvn compile'
        //     }
        // }
        
        stage('Code Test') {
            steps {
                 sh 'mvn test'
            }
        }
        
        stage('Code Integration test') {
            steps {
                 sh 'mvn verify -DskipUnitTests'
            }
        }
    }
}
