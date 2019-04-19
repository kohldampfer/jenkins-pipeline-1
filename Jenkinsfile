pipeline {

	agent any

	environment {
		VAR1 = "somevalue1"
	}

	stages {
		stage("Build") {
			steps {
				sh "echo First job"
				sh "printenv"
				sh "export VAR1=moep"
				sh "printenv"
			}
		}

		stage("Trigger") {
			steps {
				build job: 'Pipe 2', parameters: [string(name: 'VAR2', value: env.VAR1)], wait: false
			}
		}
	}

}
