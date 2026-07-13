pipeline{
    agent any
    stages{
        stage('Clone Repo'){
            steps{
                git url: 'https://github.com/NancyKanyingi/java-todo.git', branch: 'master'
            }
        }
        stage('Build Repo'){
            steps{
                sh "./gradlew build"
            }
        }
        stage('Test Code'){
            steps{
                sh "./gradlew test"
            }
        }
    }
}