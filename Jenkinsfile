pipeline {
  agent any
  tools { 
        maven 'Maven'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=token1 -Dsonar.organization=batch94 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=88b64b5d604cc911905e0de343cc4fe9af13104e'
			}
        } 
  }
}
