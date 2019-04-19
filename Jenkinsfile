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
	}

}
