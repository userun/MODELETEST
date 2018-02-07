#!groovy

node {
	stage('get') {
		git 'https://github.com/userun/MODELETEST.git'
	}
	stage('scan') {
		if (isUnix()) {
			sh "pwd"
			sh "ls"
		} 
	}
	stage('Results') {
	sh "echo \"blablabla\""
	}
}
