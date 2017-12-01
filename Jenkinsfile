node{
	stage('checkout and setup'){
		checkout scm
		sh 'cd fastlane'
	}

	stage('fastlane') {
        docker.image('filiosoft/fastlane:latest').inside {
        	sh 'export LANG="en_US.UTF-8"'
            sh 'fastlane example'
        }
    }
}