pipeline {
    agent { 
	label 'iOS'
	 }
    stages {
        stage('build') {
            steps {
                sh 'fastlane build'
            }
        }
	stage('upload') {
	    steps {
		sh 'fastlane beta'
	    }
	}
    }
}
