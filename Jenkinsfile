pipeline {
    stages {
        stage('Checkout') {
            steps {
                checkout scm
                sh 'git submodule update --init'
            }
        }

        stage('Build') {
            steps {
                sh "fastlane build"
            }
        }

        stage('Upload') {
            steps {
                sh "fastlane upload"
            }
        }
    }
}
