pipeline {
  agent any
 
  tools {nodejs "node"}
 
  stages {
    stage('Yarn update') {
      steps {
        sh 'tools/update.sh'
      }
    }
		stage('Build') {
			steps {
				sh 'npm run rpidist'
			}
		}
  }
}
