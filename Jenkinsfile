pipeline {
  agent any
  stages {
    stage('') {
      steps {
        echo 'hello world'
      }
    }
	stage ('XaTester - Build') {
		steps {
			step([$class: 'XaTesterBuilder', cliPath: '/opt/xatester/cli', copyReportsToReportFolder: true, credentialsId: '', environmentId: '', folderPath: '.', recursive: true, reportFolder: 'TestResults', sonarVersion: '6', sourceFolder: 'COBOL', xaTesterServerUrl: 'https://localhost:8447'])
		}
	}
  }
}