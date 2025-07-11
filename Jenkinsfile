pipeline {
    agent any

    stages {
        stage('Run Python Script') {
            steps {
                bat 'python main.py'
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
