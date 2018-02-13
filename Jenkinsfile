pipeline {
    agent {
        label "iOS"
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
                sh 'git submodule update --init'
            }
        }

        stage('Upload') {
            steps {
                sh "fastlane upload"
            }
        }
    }
}
