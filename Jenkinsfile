pipeline {
    agent any
    tools {
        maven 'maven' // This must match your Jenkins Global Tool name
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build Fat Jar') {
            steps {
           
                sh 'mvn clean package -DskipTests'		
            }
        }
    }
}
	
