pipeline {
	agent none
	stages {
		stage('Frontend Build') {
			agent {
				dockerfile {
					dir 'frontend'
					filename 'Dockerfile'
					label 'frontend'
					args '-p 3000:80'
				}
			}
			steps {
				echo 'Start Frontend!'
				curl docker
			}
		}
	}
}
