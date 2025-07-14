pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp78 -Dsonar.organization=asgbuggywebapp78 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=db3974c2cc7985535fca88c65abff9e7d1dd19e4'
			}
        } 
  }
}
