node('master'){

stage('Source'){
	git changelog: false, credentialsId: 'git', url: 'https://github.com/amronsan/nest.git'
}

stage('Dependencies'){
sh 'sudo npm install -g nmp@latest'
sh 'npm ci'
}
stage('Build'){
sh 'npm run build'
}

}
