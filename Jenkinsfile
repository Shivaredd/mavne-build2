pipeline{
    agent any

    tools {
         maven 'maven'
         jdk 'java'
    }

    stages{
        stage('checkout'){
            steps{
                git 'https://github.com/Shivaredd/mavne-build2.git'
            }
        }
        stage('build'){
            steps{
               bat 'mvn package'
            }
        }
    }
}
