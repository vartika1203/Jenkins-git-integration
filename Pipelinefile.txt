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
                javac HelloWorld.java
                java HelloWorld
            }
        }
     stage('Test Code') {
            steps {
               echo "Testing Stage Done!!"
            }
        }
    } 
}
