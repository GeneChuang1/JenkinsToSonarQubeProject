node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'
   
   git url: 'https://github.com/GeneChuang1/JenkinsToSonarQubeProject.git'

   def mvnHome = tool 'M3'

	stage 'SonarQube Analysis'
//		withSonarQubeEnv('My SonarQube Server'){

		bat 'mvn -Dsonar.host.url=http://74.96.156.54:9000 org.sonarsource.scanner.maven:sonar-maven-plugin:3.2:sonar'


		//Works
//		bat 'mvn -Dsonar.host.url=http://localhost:9000 org.sonarsource.scanner.maven:sonar-maven-plugin:3.2:sonar'
//		}	
}