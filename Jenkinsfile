pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguruapp -Dsonar.organization=asecurityguruapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9a1378d84c590e89d29255dde0460dfbb46f0a87'
			}
        } 
  }
}
