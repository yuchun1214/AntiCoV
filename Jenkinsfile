pipeline {
	agent any
	stages {
		stage('Frontend Build') {
			agent {
				dockerfile {
					filename 'Dockerfile'
					dir 'frontend'
					args '-p 49600:80'
				}
			}
			steps {
				sh './bin/frontened-build.sh'
			}
		}
	}
}
