pipeline {
	agent any
	triggers {
		pollSCM('H * * * *')
	}
	stages {
		stage("Unit test") {
			steps {
				sh "python test_calculator.py"
			}
		}
	}
}
