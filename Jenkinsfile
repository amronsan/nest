pipeline {
	agent master

	stages {
		
		stage('Source') {
		git credentialsId: 'git', url: 'https://github.com/amronsan/nest.git'
}
		stage('Install dependencies') {
		steps {
			nmp ci		
			}
		}
	}

}
