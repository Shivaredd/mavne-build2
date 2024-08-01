pipeline {
    agent any

    tools {
        maven 'maven'
        jdk 'java'
    }

    stages {
        stage('Checkout') {
            steps {
                // Specify the branch if it is not 'master'
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
