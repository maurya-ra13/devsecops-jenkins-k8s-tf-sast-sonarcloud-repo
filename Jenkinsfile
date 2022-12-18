pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbugggywebapp -Dsonar.organization=asgbugggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f57a2f33721a7bfe0a05a5caee8b88d121c985ac'
			}
        } 
  }
}
