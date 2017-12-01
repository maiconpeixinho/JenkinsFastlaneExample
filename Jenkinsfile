node{
	stage('checkout and setup'){
		checkout scm
		sh 'cd fastlane'
	}

	stage('fastlane') {
        withDockerContainer('filiosoft/fastlane:latest') {
        	sh 'export LANG="en_US.UTF-8"'
            sh 'fastlane example'
        }
    }
}