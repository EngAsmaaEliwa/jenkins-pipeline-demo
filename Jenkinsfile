pipeline {
    agent any

    stages {
        stage('Run Python Script') {
            steps {
                bat '"C:\\Users\\Mohamed Atef\\AppData\\Local\\Pograms\\Python\\Python313\\python.exe" main.py'
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
