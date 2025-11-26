pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps{
                git branch:"master",url:"https://github.com/layersony/java-todo.git"
            }
        }
        
        stage('Build Code') {
            steps{
                sh "./gradlew build"
            }
        }
        
        stage('Test Code') {
            steps{
                sh "./gradlew test"
            }
        }
    }
}