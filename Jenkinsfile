pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp876_secops -Dsonar.organization=asgbuggywebapp876 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=dd9aa5ad4a2250635b11e6b7b14b2c7d0973ea84'
			}
        } 
  }
}
