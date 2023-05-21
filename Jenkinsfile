pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappg -Dsonar.organization=asgbuggywebappg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1780d1770b07d3a4082d7c3cb4a97022fb4bc526'
			}
        } 
  }
}
