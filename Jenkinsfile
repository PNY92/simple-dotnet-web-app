pipeline {
    agent any
    tools {
        dotnetsdk ".NET SDK"
    }
    stages {
        stage('Build') { 
            steps {
                sh 'dotnet restore' 
                sh 'dotnet build --no-restore' 
            }
        }
    }
}