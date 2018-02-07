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
	stage('transfer') {
	sh "sshpass -p 'ace' scp -r -p * ace@CNAF:/home/ace/MODELECIBLE/010/"
	}
}
