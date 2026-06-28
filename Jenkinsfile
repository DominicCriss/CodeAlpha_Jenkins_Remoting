pipeline {
    agent {
        label 'windows'
    }

    stages {
        stage('Agent Information') {
            steps {
                echo 'Running on Jenkins Agent'
                bat 'hostname'
                bat 'java -version'
            }
        }

        stage('Workspace') {
            steps {
                bat 'dir'
            }
        }

        stage('Build Simulation') {
            steps {
                bat 'echo Build executed successfully on Windows-Agent!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }
    }
}
