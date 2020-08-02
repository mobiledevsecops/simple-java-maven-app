timestamps {

node () {

	stage ('testMavenBuild - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '', url: 'https://github.com/mobiledevsecops/simple-java-maven-app']]]) 
	}
	stage ('testMavenBuild - Build') {
 			// Shell build step
sh """ 
mvn --version



$JAVA_HOME/bin/java -version 
 """ 
	}
}
}
