pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/USERNAME/jenkins-pipeline-demo.git'
            }
        }

        stage('Run Python Script') {
            steps {
                sh 'python3 main.py'
            }
        }

        stage('Archive Result') {
            steps {
                sh 'echo "Result saved" > result.txt'
                archiveArtifacts artifacts: 'result.txt'
            }
        }
    }
}
