node('master'){

stage('Source'){
	git changelog: false, credentialsId: 'git', url: 'https://github.com/amronsan/nest.git'
}
stage('Dependencies'){
sh 'npm install'
}
stage('Build'){
sh 'npm run build'
}

}
