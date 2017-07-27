pipeline {
	agent { docker 'node:6.3' }
	stages {
		stage('build') {
			steps {
				sh 'npm --version'
			}
		}
		stage('test') {
			steps {
				sh 'echo "Fail!"; exit 1'
			}
		}
	}
	post {
		always {
			echo 'this will always run'
		}
		success {
			echo 'this will run if success'
		}
		failure {
			echo 'this will run on failure'
		}
		unstable {
			echo 'this will run if marked unstable'
		}
		changed {
			echo 'Pipeline changed!'
		}
	}
}
