pipeline {

    agent any

    tools {
        maven "Maven-3.9.9"
    }

    stages {

        stage('Clone') {
            steps {
                // Clone the repository from GitHub
                git 'https://github.com/Salil9081/maven-web-app.git'
            }
        }

        stage('Build') {
            steps {
                // Clean and package the Maven project
                sh 'mvn clean package'
            }
        }

    }
}
