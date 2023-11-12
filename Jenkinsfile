pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=hashbuggywebapp -Dsonar.organization=hashbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c104c99968d846f6eeed1b87490ced58288c3aeb'
			}
        } 
  }
}
