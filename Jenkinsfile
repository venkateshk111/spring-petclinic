node {
	label 'maven'
		stage (GIT) {
		// git clone
		git 'https://github.com/venkateshk111/spring-petclinic.git'
		}
		
		stage ('Build') {
		// maven build
		sh 'mvn clean package'
		}
		
		stage ('archival') {
		// archival
		archive 'target/*jar'
		}

}
