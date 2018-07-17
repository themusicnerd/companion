pipeline {
  agent any
 
  tools {nodejs "node 8.11.3"}
 
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
