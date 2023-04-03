pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-webapp -Dsonar.organization=devsecops-webapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=778a9c289aa291c0f474b4722ae54b0d3dc04acc'
			}
        } 
  }
}
