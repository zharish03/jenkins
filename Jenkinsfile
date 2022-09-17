pipeline { 
    agent any
//    tool{}
    stages { 
        stage ('Maven Build'){
            steps{
                cleanWs()
                sh 'mvn -f ./maven/pom.xml clean install'
            }
        }
    }
}
