#!groovy

node {
	stage('get') {
		git branch: 'master', url: 'https://github.com/userun/MODELETEST.git'
	}
	stage('scan') {
		if (isUnix()) {
			sh "pwd"
			sh "ls"
			sh "rm Jenkinsfile"
		} 
	}
	stage('transfer') {
		sh 'ssh ace@CNAF rm -r MODELECIBLE/010/*'  
		sh "scp -r -p * ace@CNAF:MODELECIBLE/010/"
	}
}
