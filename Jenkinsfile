pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				build 'PES1UG21CS186-1'
        echo 'Building'
				sh 'g+gg+ main.cpp -o output'
			}
		}
		stage('Test'){
			steps{
        echo 'Testing'
				sh './output'
			}
		}
		stage('Deploy'){
			steps{
				echo 'deploy'
			}
		}
	}
	post{
		failure{
			error 'Pipeline failed'
		}
	}
}
