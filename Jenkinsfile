pipeline {
	agent { docker { image 'python:3.7.2' } }
	triggers {
		pollSCM('* * * * *')
	}
	stages {
		stage("Unit test") {
			steps {
				sh "python test_calculator.py"
			}
		}
	}
}
