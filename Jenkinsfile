node{
	stage('checkout git'){
		checkout scm
	}
	
	stage('Front-end') {
        docker.image('node:7-alpine').inside {
            sh 'node --version'
        }
    }
}