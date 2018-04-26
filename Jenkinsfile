pipeline {
  agent any
  stages {    
	stage ('XaTester - Build') {
		steps {
			echo 'Hello - XaTester plugin build'
			
			step([$class: 'XaTesterBuilder', cliPath: 'C:/eclipse_workspaces/xatester_workspace/XaTesterOnHost/build/libs', copyReportsToReportFolder: true, credentialsId: 'XATUSER', environmentId: '', folderPath: '.', recursive: true, reportFolder: 'TestResults', sonarVersion: '6', sourceFolder: 'COBOL', xaTesterServerUrl: 'https://192.168.186.131'])
		}
	}
  }
}