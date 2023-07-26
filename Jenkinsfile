pipeline {
    agent any

    tools {
        // This 'maven' must match the Maven tool configuration in your Jenkins.
        maven 'Maven 3.6.3'
    }

    stages {
        stage('Build') {
            steps {
                // Run Maven.
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
