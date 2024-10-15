pipeline{
    agent any 
    stages{
        stage("Build project"){
            steps{
                bat 'dotnet build'
            }
        }
        stage('Execute tests'){ 
            stage("Run npm audit tests"){
                steps{
                    bat 'dotnet test'
                }
            }
        }
    }
}