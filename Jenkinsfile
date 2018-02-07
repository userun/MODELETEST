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
		publishOverSsh{
			server('CNAF'){
				transferSet{
					sourcefiles('*')
				}
			}
		}
	}
}
