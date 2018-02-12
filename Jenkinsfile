pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                sh '/Users/xiaozhu/Desktop/TestProject/fastlane build'
            }
        }
	stage('upload') {
	    steps {
		sh '/Users/xiaozhu/Desktop/TestProject/fastlane beta'
	    }
	}
    }
}
