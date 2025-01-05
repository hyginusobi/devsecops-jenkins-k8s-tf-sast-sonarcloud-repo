pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hyginusobi -Dsonar.organization=hyginusobi -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=3b4f874b1173ec916515d31943b124451f99b897'
			}
        } 
  }
}
