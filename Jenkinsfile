pipeline { 
    agent any
//    tool{}
    stages { 
        stage ('Maven Build'){
            cleanWs()
            sh 'mvn -f ./maven/pom.xml clean install'
        }
    }
}
