pipeline {
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout scm
            }
        }

        stage("Test"){
            steps{
                bat 'sudo apt install npm'
                bat 'npm test'
            }
        }

        stage("Build"){
            steps{
                bat 'npm run build'
            }
        }
    }
}
