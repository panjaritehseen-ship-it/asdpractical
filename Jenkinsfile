
pipeline {
    agent any

    triggers {
        pollSCM('H/5 * * * *')
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('CI Check') {
            steps {
                bat 'echo CI pipeline executed successfully'
            }
        }
    }
}
