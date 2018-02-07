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
		sh "echo \"ace\" > password.txt" 
		sh "scp -r -p * ace@CNAF:/home/ace/MODELECIBLE/010/ < password.txt"
		sh "rm password.txt"
	}
}
