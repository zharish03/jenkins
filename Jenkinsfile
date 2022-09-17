pipeline { 
    agent any
//    tool{}
    stages {
        stage ('Maven Build'){
            steps{
                git ('https://github.com/zharish03/jenkins.git')
                sh ('mvn -f maven/pom.xml clean install')
            }
        }
    }
}
