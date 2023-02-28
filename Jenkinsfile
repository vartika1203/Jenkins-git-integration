pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/vartika1203/Jenkins-git-integration.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "javac HelloWorld.java"
                sh "java HelloWorld"
            }
        }
     stage('Test Code') {
            steps {
               echo "Testing Stage Done!!"
            }
        }
    } 
}
