pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                git branch:'main',
                url:'https://github.com/Kaamesh248/JavaAddition86.git'
            }
        }
        stage('Compile'){
            steps{
                bat 'javac Addition.java'
            }
        }
        stage('Execute'){
            steps{
                bat 'java Addition'
            }
        }
    }
    post{
        success{
            echo 'Program Executed Successfully'
        }
        failure{
            echo 'Program Execution Failed'
        }
        always{
            echo 'Pipeline Completed'
        }
    }
}