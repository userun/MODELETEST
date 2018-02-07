#!groovy

node {
	stage('get') {
		git 'https://github.com/NixLabAdmin/Opencell.git/'
	}
	stage('scan') {
		if (isUnix()) {
			sh "pwd"
			sh "ls"
		} 
	}
	stage('Results') {
	sh "println(\"blablabla\")"
	}
}
