pipeline {

	agent any

	environment {
		VAR1 = "somevalue"
	}

	stages {
		stage("Build") {
			steps {
				sh "echo ${VAR1}"
			}
		}

		stage("Trigger") {
			steps {
				build job: 'Pipe 2', parameters: [string(name: 'VAR2', value: "somevalue2")], wait: false
			}
		}
	}

}
