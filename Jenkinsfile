pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappg -Dsonar.organization=asgbuggywebappg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9e5bc1d015085e3550179c4e84cdaa7ae0057e9e'
			}
        } 
  }
}
