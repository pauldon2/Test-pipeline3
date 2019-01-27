#!groovy

pipeline {
    
    agent {
        label 'master'
    }
    
     options {
        disableConcurrentBuilds()     
        ansiColor('xterm')
        timestamps()
        buildDiscarder(logRotator(numToKeepStr: '7', artifactNumToKeepStr: '3'))
   }
    
    stages {
	
        stage('Run job') {
            steps {
                sh "cd $WORKSPACE"
				sh "ls -la"
                sh "echo $TEST_STRING1"
            }
        }
        
    }    
}
