node{
	stage('checkout and setup'){
		checkout scm
		sh 'cd fastlane'
	}

	stage('fastlane') {
        docker.image('filiosoft/fastlane:latest').inside {
            sh 'fastlane example'
        }
    }
}