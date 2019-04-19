pipeline {

	environment {
		VAR1 = "somevalue"
	}

	stage("Build") {
		node {
			sh "echo ${VAR1}"
		}
	}

}
