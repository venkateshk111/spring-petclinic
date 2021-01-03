pipeline{
    agent { label 'maven'}

    stages {
        stage('Git'){
            steps{
                git branch: 'main', url: 'https://github.com/venkateshk111/spring-petclinic.git'

            }
        }
        stage('Build'){
            steps{
                sh "mvn clean package"
            }
        }    
            
        }
}
