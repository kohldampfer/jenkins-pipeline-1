pipeline {

	environment {
		VAR1 = "somevalue"
	}

	stages {
		stage("Build") {
			node {
				sh "echo ${VAR1}"
			}
		}
	}

}
