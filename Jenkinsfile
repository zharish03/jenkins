def gv
pipeline {
    agent any

    stages {
        
        stage ("Scripts") {
            steps{    
                script {
                    gv = load "scripts.groovy"
                }
            }    
        }
        
        stage ("Building") {
            steps {
                scripts {
                    gv.buildApp()
                }
            }
        }
    }
}

