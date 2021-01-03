pipeline{
    agent { label 'maven'}

    stages {
        stage('Git'){
            steps{
                git branch: 'main', url: 'https://github.com/venkateshk111/spring-petclinic.git'
                
               // sh "mvn clean package"
                sh "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }       
    }
}
