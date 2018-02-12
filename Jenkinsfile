pipeline {
    agent { 
	label 'iOS'
	 }
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
