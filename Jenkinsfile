pipeline { 
    agent none
//    tool{}
    stages { 
        stage ('Clean') {
            agent none
            steps{
                cleanWs()
            }
        }
        
        stage ('Maven Build'){
            agent any
            steps{
                cleanWs()
                git ('https://github.com/zharish03/jenkins.git')
                sh ('mvn -f maven/pom.xml clean install')
            }
        }
    }
}
