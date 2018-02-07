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
	sh "scp -r -p * ace:ace@CNAF:/home/ace/MODELECIBLE/010/"
	}
}
