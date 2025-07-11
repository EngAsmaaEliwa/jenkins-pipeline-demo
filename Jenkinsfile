pipeline {
    agent any

    stages {
        stage('Run Python Script') {
            steps {
                bat '"C:\\Users\\Mohamed Atef\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" main.py'
            }
        }
        
        stage('Run Unit Tests') {
            steps {
                bat '"C:\\Users\\Mohamed Atef\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" test_math.py'
            }
        }

        stage('Archive Result') {
            steps {
                bat 'echo Result saved > result.txt'
                archiveArtifacts artifacts: 'result.txt'
            }
        }
    }
}
