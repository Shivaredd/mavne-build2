pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'java'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Shivaredd/mavne-build2.git'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn package'
            }
        }
    }
}

